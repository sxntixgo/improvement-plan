# Track 6: Docker Essentials

**Duration:** 1 week | **Total:** ~18 hours
**Weekly breakdown:** 8 hrs weekdays + 5 hrs Sat + 5 hrs Sun
**Priority:** HIGH
**Goal:** Container fundamentals for development and deployment

-----

## Why After Go?

Docker is foundational infrastructure that you'll use across all future tracks:

- **Python projects** (Weeks 9-18): Containerize TDD projects, reproducible dev environments
- **AI/ML work** (Weeks 19-26): Model serving, isolated ML environments, GPU containers
- **Security testing**: Isolated vulnerable app environments, CTF lab setups
- **Modern workflows**: CI/CD, deployment, collaboration

Learning Docker now (Week 7) means:
- Available immediately for Python Core projects
- Ready for ML deployment and security labs
- One concentrated week for better retention vs scattered learning

-----

## Resources

|Resource                          |Cost|Type              |
|----------------------------------|----|------------------|
|Docker Official Documentation     |FREE|Comprehensive     |
|Docker Deep Dive (Poulton)        |~$40|Optional book     |
|TechWorld with Nana (YouTube)     |FREE|Video tutorials   |
|Play with Docker (labs.play-...)  |FREE|Hands-on labs     |

**Recommended Approach:** Free resources are sufficient. Only buy Docker Deep Dive if you want a reference book.

**Total Cost This Week:** $0 (all free resources)

-----

## Weekly Breakdown

### Monday-Tuesday (6 hours): Docker Basics

**Monday (3 hours): Containers & Images**
- What are containers vs VMs?
- Docker architecture (daemon, CLI, registry)
- Images vs containers
- Docker Hub and image layers

**Hands-on:**
```bash
# Pull and run containers
docker pull nginx
docker run -d -p 8080:80 nginx
docker ps
docker stop <container-id>

# Explore images
docker images
docker inspect nginx
docker history nginx
```

**Tuesday (3 hours): Dockerfile Basics**
- Writing Dockerfiles (FROM, RUN, COPY, CMD, ENTRYPOINT)
- Building images
- Layer caching
- .dockerignore

**Hands-on:**
```dockerfile
# Simple Python app
FROM python:3.11-slim
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
CMD ["python", "app.py"]
```

**Project:** Containerize a simple Python script

-----

### Wednesday-Thursday (6 hours): Docker Compose & Networking

**Wednesday (3 hours): Docker Compose**
- Multi-container applications
- docker-compose.yml syntax
- Service dependencies
- Environment variables

**Hands-on:**
```yaml
version: '3.8'
services:
  web:
    build: .
    ports:
      - "5000:5000"
    depends_on:
      - db
  db:
    image: postgres:15
    environment:
      POSTGRES_PASSWORD: secret
    volumes:
      - db-data:/var/lib/postgresql/data
volumes:
  db-data:
```

**Thursday (3 hours): Volumes & Networking**
- Persistent data with volumes
- Bind mounts vs named volumes
- Docker networks (bridge, host, none)
- Container communication

**Hands-on:**
```bash
# Volumes
docker volume create mydata
docker run -v mydata:/data alpine

# Networks
docker network create mynetwork
docker run --network mynetwork --name app1 nginx
docker run --network mynetwork --name app2 alpine ping app1
```

-----

### Friday (3 hours): Development Workflows

**Docker for Development:**
- Dev containers vs production containers
- Hot reloading with bind mounts
- Debugging inside containers
- Multi-stage builds for smaller images

**Multi-stage Dockerfile:**
```dockerfile
# Build stage
FROM python:3.11 AS builder
WORKDIR /app
COPY requirements.txt .
RUN pip install --user -r requirements.txt

# Production stage
FROM python:3.11-slim
WORKDIR /app
COPY --from=builder /root/.local /root/.local
COPY . .
ENV PATH=/root/.local/bin:$PATH
CMD ["python", "app.py"]
```

**Company Workflow Questions:**
- Does your team use Docker? What's the standard setup?
- Any internal Docker registries?
- Docker Compose conventions?
- Security policies (image scanning, approved base images)?

-----

### Weekend (6 hours): Security Labs & Practice

**Saturday (3 hours): Security Use Cases**
- Running vulnerable apps for testing (DVWA, WebGoat, juice-shop)
- Isolated testing environments
- Container escape scenarios (awareness)
- Docker security best practices

**Hands-on:**
```bash
# Run OWASP Juice Shop for security testing
docker run -d -p 3000:3000 bkimminich/juice-shop

# Run vulnerable web app (DVWA)
docker run -d -p 8080:80 vulnerables/web-dvwa

# Quick CTF environment
docker run -d -p 2222:22 ctf-challenges/pwn-basic
```

**Sunday (3 hours): Build Your Own Lab**
- Create a Docker Compose lab with vulnerable services
- Practice: Web app + database + reverse proxy
- Document your setup for future security testing

**Example Lab Setup:**
```yaml
version: '3.8'
services:
  vulnerable-app:
    image: bkimminich/juice-shop
    ports:
      - "3000:3000"

  dvwa:
    image: vulnerables/web-dvwa
    ports:
      - "8080:80"

  postgres:
    image: postgres:15
    environment:
      POSTGRES_PASSWORD: vulnerable
    ports:
      - "5432:5432"
```

-----

## Projects & Outputs

|Project                     |Output                              |Share    |
|----------------------------|-------------------------------------|---------|
|Containerized Python app    |Dockerfile + docker-compose.yml     |GitHub   |
|Security testing lab        |Multi-container vulnerable app setup|GitHub   |
|Docker learnings            |Best practices and gotchas          |Blog post|

-----

## Essential Docker Commands

**Images:**
```bash
docker images              # List images
docker pull <image>        # Download image
docker build -t name .     # Build from Dockerfile
docker rmi <image>         # Remove image
docker tag <image> <tag>   # Tag image
```

**Containers:**
```bash
docker ps                  # List running containers
docker ps -a               # List all containers
docker run <image>         # Create and start container
docker start/stop <id>     # Start/stop container
docker rm <id>             # Remove container
docker logs <id>           # View logs
docker exec -it <id> bash  # Shell into container
```

**Compose:**
```bash
docker-compose up          # Start services
docker-compose up -d       # Start in background
docker-compose down        # Stop and remove
docker-compose logs        # View logs
docker-compose ps          # List services
```

**Cleanup:**
```bash
docker system prune        # Remove unused containers/images/networks
docker volume prune        # Remove unused volumes
```

-----

## Docker Security Best Practices

**For Development:**
- Don't run containers as root (use USER directive)
- Scan images for vulnerabilities (docker scan or Trivy)
- Use official images from Docker Hub
- Keep base images updated
- Don't store secrets in images (use env vars or secrets)

**Dockerfile Best Practices:**
```dockerfile
# Good: Specific version, non-root user, minimal layers
FROM python:3.11-slim
RUN useradd -m appuser
WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
USER appuser
CMD ["python", "app.py"]

# Bad: Latest tag, running as root, many layers
FROM python:latest
RUN apt-get update
RUN apt-get install -y vim
RUN apt-get install -y curl
COPY . .
RUN pip install flask
CMD ["python", "app.py"]
```

-----

## Deliverables

**By end of Week 7, you should have:**
- [ ] Completed Docker basics (images, containers, Dockerfile)
- [ ] Written docker-compose.yml for multi-container apps
- [ ] Understand volumes and networking
- [ ] Built at least one containerized Python app
- [ ] Set up a security testing lab with Docker Compose
- [ ] Comfortable using Docker for development

**NOT expected:**
- ❌ Kubernetes (that's for later)
- ❌ Docker Swarm
- ❌ Advanced orchestration
- ❌ Production deployment at scale

-----

## Week 7 Checklist

### Learning
- [ ] Understand containers vs images vs VMs
- [ ] Write Dockerfiles with best practices
- [ ] Use Docker Compose for multi-container apps
- [ ] Understand volumes and networking
- [ ] Know security best practices

### Practice
- [ ] Containerize a Python application (3+ hours)
- [ ] Build multi-container app with Compose (3+ hours)
- [ ] Set up security testing lab (3+ hours)

### Work Integration
- [ ] Ask team about Docker usage
- [ ] Understand company's container workflow
- [ ] Identify where Docker helps your work

-----

## What's Next?

**Week 8: LLM Security Primer**
- Read Wilson's book
- Docker available for running vulnerable LLM apps
- Container isolation for testing prompt injections

**Weeks 9-18: Python Core**
- Containerize your TDD projects
- Docker Compose for Django apps + PostgreSQL
- Reproducible dev environments

**Weeks 19-26: AI/ML Security**
- ML model serving in containers
- GPU containers for model training
- Isolated environments for testing adversarial attacks

**Ongoing:**
- Use Docker for all projects
- Security testing labs with containers
- CI/CD integration (later tracks)

-----

## Tips for Success

**For Learning:**
1. Hands-on practice > reading documentation
2. Start with simple apps, gradually add complexity
3. Use Docker Desktop (GUI) initially if helpful
4. Read error messages carefully - Docker errors are usually clear
5. Clean up regularly (docker system prune) to save disk space

**For Development:**
1. Use .dockerignore (like .gitignore for Docker)
2. Leverage layer caching (put changing files last)
3. Multi-stage builds for production images
4. Bind mounts for hot reloading during development
5. Named volumes for persistent data

**For Security:**
1. Always use specific image tags (not :latest)
2. Scan images before use
3. Run containers as non-root
4. Don't expose unnecessary ports
5. Use Docker for isolated testing environments

-----

## Common Pitfalls

**Avoid these mistakes:**
1. **Not cleaning up**: Docker uses lots of disk space - prune regularly
2. **Using :latest tag**: Always specify versions (python:3.11, not python:latest)
3. **Running as root**: Use USER directive in Dockerfile
4. **Bloated images**: Use slim/alpine variants, multi-stage builds
5. **Secrets in images**: Use environment variables or Docker secrets
6. **Ignoring .dockerignore**: Copying unnecessary files (node_modules, .git)

-----

## Cost Summary

**This week: $0**
- All resources are free
- Optional: Docker Deep Dive book (~$40) - only if you want reference

-----

## Success Criteria

**You're ready to move on when:**
- ✅ Can write Dockerfiles for Python apps
- ✅ Can use Docker Compose for multi-container setups
- ✅ Understand volumes, networks, and bind mounts
- ✅ Built and containerized at least one project
- ✅ Set up a security testing lab with Docker
- ✅ Can debug issues inside containers

**Stretch goals:**
- Multi-stage builds for smaller images
- Custom Docker networks
- Docker volume backups
- Container health checks
