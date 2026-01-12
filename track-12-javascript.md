# Track 12: JavaScript/TypeScript

**Duration:** 20 weeks | **Hours/week:** 18 | **Priority:** MEDIUM
**Goal:** Full-stack JS/TS for security tooling and modern web applications

**Learning Path:** JavaScript Fundamentals → TypeScript → Security

**Weekly Schedule:**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

-----

## Why JavaScript → TypeScript?

**TypeScript is essential for modern AI/ML tooling:**
- LangChain, Vercel AI SDK, and many LLM tools use TypeScript
- Modern web apps (React/Next.js) use TypeScript
- Better code reading with type definitions
- But you need JavaScript fundamentals first

**Learning Path:**
1. **Weeks 47-52:** Pure JavaScript (foundation)
2. **Weeks 53-58:** TypeScript for Node.js/Express
3. **Weeks 59-62:** Advanced TypeScript patterns
4. **Weeks 63-66:** Security in both JS and TS

-----

## Phase Overview

|Phase|Weeks|Focus                            |Primary Resource              |
|-----|-----|---------------------------------|------------------------------|
|1    |47-52|JavaScript Fundamentals          |Eloquent JavaScript           |
|2    |53-58|Node.js & Express with TypeScript|TypeScript Handbook + Brown   |
|3    |59-62|TypeScript Advanced Patterns     |TypeScript Handbook + Patterns|
|4    |63-66|Security Focus (JS & TS)         |OWASP + Hands-on              |

-----

## Resources

### Books You Already Own

|Book                                         |Phase|Type          |
|---------------------------------------------|-----|--------------|
|Eloquent JavaScript (Haverbeke)              |1    |Project-driven|
|Web Development with Node and Express (Brown)|2    |Project-driven|
|You Don't Know JS 1st edition (Simpson)      |1,4  |Deep dive     |
|Node.js: The Comprehensive Guide (Springer)  |2-4  |Reference     |

### Free Resources (TypeScript)

|Resource                    |URL                                        |Type          |Cost|
|----------------------------|-------------------------------------------|--------------|----|
|TypeScript Handbook         |typescriptlang.org/docs/handbook           |Official docs |FREE|
|TypeScript Deep Dive        |basarat.gitbook.io/typescript              |Comprehensive |FREE|
|Execute Program (TypeScript)|executeprogram.com                         |Interactive   |~$20/mo (optional)|
|Matt Pocock TypeScript      |YouTube: @mattpocockuk                     |Video tutorials|FREE|
|Total TypeScript            |totaltypescript.com (free tutorials)       |Hands-on      |FREE|

### Paid Resources (Optional)

|Book/Course                    |Cost   |Worth It?                        |
|-------------------------------|-------|---------------------------------|
|Programming TypeScript (Cherny)|~$40   |✅ Yes - very practical, examples|
|Node.js Design Patterns (3rd ed)|~$45  |✅ Yes - includes TypeScript     |
|Execute Program subscription   |$20/mo |⚠️ Optional - excellent but pricey|

**Recommended:** Stick with FREE resources (TypeScript Handbook is excellent). Only buy *Programming TypeScript* if you want a structured reference.

-----

## Phase 1: JavaScript Fundamentals (Weeks 47-52)

**Goal:** Master JavaScript before TypeScript
**Primary Resource:** Eloquent JavaScript, 4th Edition (FREE at eloquentjavascript.net)

### Week 47: JavaScript Basics

**Eloquent JavaScript: Chapters 1-3 (18 hours)**

**Monday-Tuesday (6 hours): Chapter 1 & 2**
- Chapter 1: Values, Types, and Operators (2 hours)
  - Numbers, strings, booleans, operators
  - Type coercion (understand `==` vs `===`)
- Chapter 2: Program Structure (4 hours)
  - Variables (let, const, var)
  - Control flow (if, while, for)
  - Functions basics
  - Exercises: FizzBuzz, chessboard

**Wednesday-Thursday (6 hours): Chapter 3**
- Chapter 3: Functions (6 hours)
  - Function declarations vs expressions
  - Arrow functions
  - Scope and closures
  - Recursion
  - Exercises: Minimum, recursion, bean counting

**Friday (3 hours): Practice & Consolidation**
- JavaScript30: Day 1-3 challenges
- Build: Simple calculator with functions

**Weekend (3 hours): Deep Dive**
- YDKJS 1st ed: Chapter 1-2 (Scope overview)
- Namaste JavaScript: Episode 1-5 (YouTube)

-----

### Week 48: Data Structures & Functions

**Eloquent JavaScript: Chapters 4-5 (18 hours)**

**Monday-Tuesday (6 hours): Chapter 4**
- Chapter 4: Data Structures: Objects and Arrays (6 hours)
  - Arrays and array methods (map, filter, reduce)
  - Objects and properties
  - Mutability
  - JSON
  - Exercises: Sum of range, reversing arrays, deep comparison

**Wednesday-Friday (9 hours): Chapter 5**
- Chapter 5: Higher-Order Functions (9 hours)
  - Abstraction with functions
  - Passing functions as values
  - Array methods deep dive (forEach, map, filter, reduce, find, some, every)
  - Exercises: Flattening, your own loop, everything

**Weekend (3 hours): Practice**
- JavaScript30: Day 4-6 (Array Cardio)
- Build: Data transformation pipeline for JSON

-----

### Week 49: Objects & Project

**Eloquent JavaScript: Chapters 6-7 (18 hours)**

**Monday-Wednesday (9 hours): Chapter 6**
- Chapter 6: The Secret Life of Objects (9 hours)
  - Object-oriented programming in JavaScript
  - Prototypes
  - Classes (ES6)
  - Getters, setters, and statics
  - Exercises: A vector type, groups, iterable groups

**Thursday-Weekend (9 hours): Chapter 7 - Project**
- Chapter 7: Project: A Robot (9 hours)
  - Build delivery robot simulation
  - Graph theory basics
  - Pathfinding
  - Performance measurement
  - **Deliverable:** Working robot simulation (GitHub)

-----

### Week 50: Error Handling & Regex

**Eloquent JavaScript: Chapters 8-9 (18 hours)**

**Monday-Wednesday (9 hours): Chapter 8**
- Chapter 8: Bugs and Errors (9 hours)
  - Debugging techniques
  - Strict mode
  - Exceptions (try/catch/finally)
  - Error propagation
  - Assertions and testing basics
  - Exercises: Retry, the locked box

**Thursday-Weekend (9 hours): Chapter 9**
- Chapter 9: Regular Expressions (9 hours)
  - Regex syntax and patterns
  - Character classes, groups, and repetition
  - Regex methods (test, exec, match, replace)
  - Security: regex DOS attacks
  - Exercises: Regexp golf, quoting style, numbers again

-----

### Week 51: Modules & Async

**Eloquent JavaScript: Chapters 10-11 (18 hours)**

**Monday-Wednesday (9 hours): Chapter 10**
- Chapter 10: Modules (9 hours)
  - ES modules (import/export)
  - CommonJS (require/module.exports)
  - Packages and npm basics
  - Module design patterns
  - Exercises: A modular robot

**Thursday-Weekend (9 hours): Chapter 11**
- Chapter 11: Asynchronous Programming (9 hours)
  - Callbacks, callback hell
  - Promises (then, catch, finally)
  - Async/await
  - Event loop understanding
  - Exercises: Tracking scalpel, building Promise.all

**Important:** This async knowledge is CRITICAL for TypeScript + Node.js

-----

### Week 52: Programming Language Project

**Eloquent JavaScript: Chapters 12-13 (18 hours)**

**Entire Week: Chapter 12 & 13 - Project**
- Chapter 12: Project: A Programming Language (12 hours)
  - Parser implementation
  - Evaluator
  - Special forms
  - The environment
  - Build a mini programming language (Egg)

- Chapter 13: JavaScript and Performance (6 hours)
  - Performance optimization
  - Memory management
  - Profiling tools

**Deliverable:** Working Egg interpreter (GitHub + blog post)

-----

## Phase 2: Node.js & Express with TypeScript (Weeks 53-58)

**Goal:** Learn Node.js/Express directly in TypeScript
**Primary Resources:** TypeScript Handbook + Web Development with Node and Express (adapted to TS)

### Week 53: TypeScript Fundamentals + Node.js Setup

**Monday-Wednesday (9 hours): TypeScript Basics**

**TypeScript Handbook:**
- **The Basics** (2 hours)
  - Static type checking
  - Types vs values
  - TypeScript compiler (tsc)
- **Everyday Types** (3 hours)
  - Primitives (string, number, boolean)
  - Arrays and tuples
  - Objects and interfaces
  - Union types
  - Type aliases
  - Literal types
- **Narrowing** (2 hours)
  - typeof guards
  - Truthiness narrowing
  - Equality narrowing
  - The `in` operator narrowing
- **Functions** (2 hours)
  - Function type expressions
  - Call signatures
  - Optional and default parameters
  - Function overloads

**Thursday-Weekend (9 hours): Node.js with TypeScript**

**Setup:**
```bash
mkdir node-ts-project
cd node-ts-project
npm init -y
npm install -D typescript @types/node ts-node nodemon
npx tsc --init
```

**Configure tsconfig.json:**
```json
{
  "compilerOptions": {
    "target": "ES2022",
    "module": "commonjs",
    "outDir": "./dist",
    "rootDir": "./src",
    "strict": true,
    "esModuleInterop": true,
    "skipLibCheck": true
  }
}
```

**Build:**
- Simple TypeScript Node.js CLI tool
- File system operations with proper types
- Error handling with TypeScript
- **Practice:** Convert Week 47-52 JS projects to TypeScript

**Reference:** Node.js: The Comprehensive Guide (Springer) - Chapters on Node.js basics

-----

### Week 54: Express with TypeScript

**Web Development with Node and Express (Brown) - Chapters 1-6, adapted to TypeScript**

**Monday-Tuesday (6 hours): Express Setup**
- Chapter 1: Introducing Express (1 hour)
- Chapter 2: Getting Started with Node (1 hour)
- Chapter 3: Saving Time with Express (2 hours)
- Chapter 4: Tidying Up (2 hours)

**TypeScript Setup:**
```bash
npm install express
npm install -D @types/express
```

**Wednesday-Friday (9 hours): Routing & Middleware**
- Chapter 5: Quality Assurance (3 hours)
  - Testing with Jest + TypeScript
  - Type-safe testing
- Chapter 6: The Request and Response Objects (6 hours)
  - Request types
  - Response types
  - Type-safe middleware

**TypeScript Patterns:**
```typescript
import { Request, Response, NextFunction } from 'express';

interface CustomRequest extends Request {
  user?: {
    id: string;
    email: string;
  };
}

const authMiddleware = (
  req: CustomRequest,
  res: Response,
  next: NextFunction
) => {
  // Type-safe middleware
};
```

**Weekend (3 hours): Project Start**
- Build: REST API with Express + TypeScript
- Type-safe routes and handlers

-----

### Week 55: Templates & Forms with TypeScript

**Web Development with Node and Express - Chapters 7-10**

**Monday-Wednesday (9 hours): Templating**
- Chapter 7: Templating with Handlebars (4 hours)
  - Type-safe view rendering
  - Typed context objects
- Chapter 8: Form Handling (3 hours)
  - Request body typing
  - Validation with zod or joi
- Chapter 9: Cookies and Sessions (2 hours)
  - Type-safe session data

**TypeScript Validation:**
```typescript
import { z } from 'zod';

const UserSchema = z.object({
  email: z.string().email(),
  password: z.string().min(8),
});

type User = z.infer<typeof UserSchema>;
```

**Thursday-Weekend (9 hours): Middleware Deep Dive**
- Chapter 10: Middleware (4 hours)
  - Type-safe middleware chains
  - Error handling middleware with types
- Practice: Build authentication middleware (5 hours)

**Project:** Type-safe Express app with auth

-----

### Week 56: Database Integration with TypeScript

**Web Development with Node and Express - Chapters 13-14**

**Monday-Wednesday (9 hours): Database Setup**
- Chapter 13: Persistence (5 hours)
  - MongoDB with TypeScript (Mongoose + types)
  - Or PostgreSQL with Prisma (recommended)
- Prisma setup (4 hours):
  - Schema definition
  - Type generation
  - CRUD operations with full type safety

**Prisma Example:**
```typescript
// schema.prisma generates types automatically
import { PrismaClient } from '@prisma/client';

const prisma = new PrismaClient();

// Fully typed database operations
const user = await prisma.user.create({
  data: {
    email: 'test@example.com',
    name: 'Test User',
  },
});
```

**Thursday-Weekend (9 hours): REST APIs**
- Chapter 14: Routing (4 hours)
  - Type-safe route handlers
  - RESTful API design with TypeScript
- Build: Complete CRUD API with TypeScript + Prisma (5 hours)

**Project:** Todo API with full type safety

-----

### Week 57: Authentication & Sessions

**Web Development with Node and Express - Chapters 18-19**

**Monday-Wednesday (9 hours): Authentication**
- Chapter 18: Security (5 hours)
  - bcrypt with types
  - JWT with typed payloads
  - HTTPS and security headers
- TypeScript JWT patterns (4 hours):

```typescript
import jwt from 'jsonwebtoken';

interface TokenPayload {
  userId: string;
  email: string;
}

const token = jwt.sign(
  { userId: '123', email: 'user@example.com' } as TokenPayload,
  process.env.JWT_SECRET!
);

const decoded = jwt.verify(token, process.env.JWT_SECRET!) as TokenPayload;
```

**Thursday-Weekend (9 hours): Sessions & Authorization**
- Chapter 19: Third-Party APIs (3 hours)
  - OAuth with TypeScript
  - Type-safe API clients
- Build: Complete auth system (6 hours)
  - Registration, login, logout
  - Protected routes
  - JWT refresh tokens

**Project:** Authentication system with TypeScript

-----

### Week 58: Production & Deployment

**Monday-Wednesday (9 hours): Production Best Practices**

**TypeScript Handbook:**
- **More on Functions** (2 hours)
  - Generic functions
  - Function constraints
- **Object Types** (2 hours)
  - Optional properties
  - Readonly properties
  - Index signatures
  - Extending types
- **Type Manipulation** (3 hours)
  - Generics
  - Keyof type operator
  - Typeof type operator
  - Conditional types
  - Mapped types
  - Template literal types
- **Classes** (2 hours)
  - Class members
  - Member visibility
  - Generic classes

**Thursday-Weekend (9 hours): Deployment**
- Production build setup
- Environment variables with type safety
- Docker with TypeScript
- Deployment to Vercel/Railway/Fly.io
- **Project:** Deploy your Express + TypeScript API

**Deliverable:** Production-ready REST API with full type safety (GitHub + blog post)

-----

## Phase 3: TypeScript Advanced Patterns (Weeks 59-62)

**Goal:** Master TypeScript for complex applications and security tooling

### Week 59: Advanced Types & Patterns

**Monday-Wednesday (9 hours): Advanced Type Features**

**TypeScript Handbook:**
- **Creating Types from Types** (3 hours)
  - Generics deep dive
  - Keyof, typeof operators
  - Indexed access types
  - Conditional types
  - Mapped types
  - Template literal types

**Advanced Patterns:**
```typescript
// Conditional types for API responses
type ApiResponse<T> = T extends { error: any }
  ? { success: false; error: string }
  : { success: true; data: T };

// Template literal types for routes
type HTTPMethod = 'GET' | 'POST' | 'PUT' | 'DELETE';
type Route = `/${string}`;
type Endpoint = `${HTTPMethod} ${Route}`;

// Mapped types for readonly versions
type Readonly<T> = {
  readonly [P in keyof T]: T[P];
};
```

**Thursday-Weekend (9 hours): Type Guards & Narrowing**
- **Handbook: Narrowing (deep dive)** (4 hours)
  - Custom type guards
  - Discriminated unions
  - Never type
  - Exhaustiveness checking
- **Practice:** Build type-safe API client (5 hours)

**Project:** Type-safe SDK for external API

-----

### Week 60: Design Patterns in TypeScript

**Monday-Friday (15 hours): Node.js Design Patterns**

**If you buy Node.js Design Patterns (3rd edition - includes TypeScript):**
- Covers common patterns in TypeScript
- Factory, Singleton, Proxy, Decorator patterns
- Async patterns with types

**FREE Alternative - Refactoring Guru + TypeScript:**
- Factory Pattern (2 hours)
- Builder Pattern (2 hours)
- Singleton Pattern (2 hours)
- Observer Pattern (2 hours)
- Strategy Pattern (2 hours)
- Decorator Pattern (2 hours)
- Dependency Injection (3 hours)

**Each pattern:**
1. Understand pattern in JavaScript
2. Add TypeScript types
3. Build example implementation

**Weekend (3 hours): Apply Patterns**
- Refactor Week 58 project with design patterns
- Add dependency injection
- Add strategy pattern for authentication

-----

### Week 61: Testing & Error Handling

**Monday-Wednesday (9 hours): Testing with TypeScript**

**Jest + TypeScript:**
```bash
npm install -D jest ts-jest @types/jest
npx ts-jest config:init
```

**Topics:**
- Unit testing with type safety (3 hours)
- Integration testing (3 hours)
- Mocking with types (2 hours)
- Test coverage (1 hour)

**Type-safe Testing:**
```typescript
describe('UserService', () => {
  it('should create user with valid data', async () => {
    const userData: CreateUserDto = {
      email: 'test@example.com',
      password: 'password123',
    };

    const user = await userService.create(userData);

    expect(user).toMatchObject<User>({
      id: expect.any(String),
      email: userData.email,
      createdAt: expect.any(Date),
    });
  });
});
```

**Thursday-Weekend (9 hours): Error Handling**
- Custom error types (3 hours)
- Result types (Option/Result pattern) (3 hours)
- Error boundaries (2 hours)
- **Practice:** Add comprehensive error handling to projects (1 hour)

**Result Type Pattern:**
```typescript
type Result<T, E = Error> =
  | { success: true; value: T }
  | { success: false; error: E };

async function createUser(data: CreateUserDto): Promise<Result<User>> {
  try {
    const user = await db.user.create({ data });
    return { success: true, value: user };
  } catch (error) {
    return { success: false, error: error as Error };
  }
}
```

-----

### Week 62: Real-World TypeScript Project

**Entire Week (18 hours): Capstone Project**

**Build: LLM Security Testing Tool in TypeScript**

**Features:**
- CLI tool for testing prompt injection
- Type-safe API clients for OpenAI/Anthropic
- Test case management
- Results reporting
- Docker containerized

**Tech Stack:**
- TypeScript
- Node.js
- Commander.js for CLI (typed)
- Zod for validation
- Prisma for test case storage
- Jest for testing

**Architecture:**
```typescript
interface LLMProvider {
  name: string;
  sendPrompt(prompt: string): Promise<string>;
}

interface TestCase {
  id: string;
  prompt: string;
  expectedBehavior: 'reject' | 'sanitize' | 'accept';
  category: 'injection' | 'jailbreak' | 'exfiltration';
}

interface TestResult {
  testCaseId: string;
  passed: boolean;
  response: string;
  analysis: string;
}

class PromptInjectionTester {
  constructor(private provider: LLMProvider) {}

  async runTest(testCase: TestCase): Promise<TestResult> {
    // Implementation
  }
}
```

**Deliverable:**
- GitHub repo with full TypeScript codebase
- Blog post: "Building a Type-Safe LLM Security Tool"
- Published npm package (optional)

-----

## Phase 4: Security Focus (Weeks 63-66)

**Goal:** Security vulnerabilities in JavaScript and TypeScript

### Week 63: JavaScript Security Fundamentals

**Monday-Wednesday (9 hours): OWASP Top 10 for JavaScript**

**Topics:**
- XSS (Cross-Site Scripting) (3 hours)
  - DOM-based XSS
  - Reflected XSS
  - Stored XSS
- Prototype Pollution (3 hours)
  - Understanding prototypes
  - Attack vectors
  - Defensive coding
- Injection attacks (3 hours)
  - SQL injection in Node.js
  - Command injection
  - Path traversal

**Hands-on:**
```javascript
// Vulnerable code
const merge = (target, source) => {
  for (let key in source) {
    target[key] = source[key];
  }
};

// Attack
merge({}, JSON.parse('{"__proto__": {"isAdmin": true}}'));

// Now all objects have isAdmin: true!
```

**Thursday-Weekend (9 hours): Common Vulnerabilities**
- SSRF (Server-Side Request Forgery) (2 hours)
- XXE (XML External Entities) (2 hours)
- Insecure deserialization (2 hours)
- **Practice:** Exploit vulnerable Node.js apps (3 hours)
  - DVNA (Damn Vulnerable Node Application)
  - NodeGoat

-----

### Week 64: TypeScript Security & Best Practices

**Monday-Wednesday (9 hours): TypeScript Security**

**Topics:**
- Type safety != runtime safety (3 hours)
  - Type assertions dangers
  - `any` type abuse
  - External data validation
- Input validation with Zod (3 hours)

```typescript
// Unsafe
app.post('/user', (req, res) => {
  const user = req.body; // any type!
  db.create(user); // 💥 Vulnerable
});

// Safe
const CreateUserSchema = z.object({
  email: z.string().email(),
  age: z.number().min(0).max(120),
});

app.post('/user', (req, res) => {
  const result = CreateUserSchema.safeParse(req.body);
  if (!result.success) {
    return res.status(400).json(result.error);
  }
  db.create(result.data); // ✅ Type-safe and validated
});
```

- Dependency vulnerabilities (3 hours)
  - npm audit
  - Snyk
  - Dependabot

**Thursday-Weekend (9 hours): Secure Coding Patterns**
- Authentication best practices (3 hours)
- Authorization patterns (3 hours)
- Secrets management (2 hours)
- **Practice:** Security audit of Week 58 project (1 hour)

-----

### Week 65: Security Tools & Testing

**Monday-Wednesday (9 hours): Security Testing**

**Tools:**
- ESLint security plugins (2 hours)
  - eslint-plugin-security
  - eslint-plugin-no-secrets
- SAST (Static Analysis) (2 hours)
  - SonarQube
  - Semgrep for JavaScript/TypeScript
- DAST (Dynamic Analysis) (2 hours)
  - Burp Suite with Node.js apps
  - ZAP (OWASP Zed Attack Proxy)
- **Practice:** Security testing automation (3 hours)

**Thursday-Weekend (9 hours): Building Security Tools**
- Build: SAST rule for Semgrep (4 hours)
- Build: Custom ESLint security rule (5 hours)

**Example Semgrep Rule:**
```yaml
rules:
  - id: unsafe-eval
    pattern: eval(...)
    message: "eval() is dangerous and should not be used"
    severity: ERROR
    languages: [javascript, typescript]
```

-----

### Week 66: Security Code Review & Final Project

**Monday-Wednesday (9 hours): Code Review Practice**

**Review Real-World Codebases:**
- Find vulnerabilities in open-source Node.js projects (6 hours)
  - Look for: eval usage, prototype pollution, SQL injection
  - Practice responsible disclosure
- Document findings (3 hours)

**Thursday-Weekend (9 hours): Final Security Project**

**Build: JavaScript/TypeScript Security Scanner**

**Features:**
- Scans JS/TS codebases for vulnerabilities
- Checks for:
  - Prototype pollution patterns
  - eval/Function usage
  - Unsafe dependencies
  - Hardcoded secrets
- Generates security report
- CLI tool with TypeScript

**Tech Stack:**
- TypeScript
- AST parsing (@babel/parser, @typescript-eslint/parser)
- Pattern matching
- Report generation

**Deliverable:**
- Security scanner tool (GitHub)
- Blog post: "Building a JavaScript Security Scanner in TypeScript"
- 5+ vulnerability findings in real projects

-----

## Projects & Outputs

|Project                          |Week   |Output                               |Share    |
|---------------------------------|-------|-------------------------------------|---------|
|Egg Programming Language         |52     |Interpreter in JavaScript            |GitHub   |
|Type-safe REST API               |56-58  |Express + TypeScript + Prisma        |GitHub   |
|LLM Security Testing Tool        |62     |CLI tool in TypeScript               |GitHub + npm|
|Custom Semgrep Rule              |65     |Security detection rule              |GitHub   |
|JavaScript Security Scanner      |66     |AST-based security scanner           |GitHub   |
|JS/TS Security Cheatsheet        |63-66  |Personal reference doc               |Blog post|

-----

## Code Review Checklist

### JavaScript Vulnerabilities
- [ ] Prototype pollution vectors?
- [ ] eval() or Function() usage?
- [ ] child_process with unsanitized input?
- [ ] JSON.parse on untrusted input?
- [ ] Missing input validation?
- [ ] Hardcoded secrets?
- [ ] DOM-based XSS sources/sinks?
- [ ] Event loop blocking?

### TypeScript-Specific
- [ ] Excessive use of `any` type?
- [ ] Unsafe type assertions (`as` keyword)?
- [ ] Missing runtime validation for external data?
- [ ] Non-null assertions (!) without checks?
- [ ] Missing null/undefined checks?

### Node.js Security
- [ ] Vulnerable dependencies (npm audit)?
- [ ] Unsafe deserialization?
- [ ] Path traversal in file operations?
- [ ] SSRF in HTTP clients?
- [ ] SQL injection (check parameterization)?
- [ ] Proper error handling (no info leakage)?

-----

## Checkpoint

**By the end of Track 12, you should be able to:**

### JavaScript
- ✅ Write modern JavaScript with ES6+ features
- ✅ Understand closures, prototypes, and the event loop
- ✅ Build full-stack applications with Node.js/Express
- ✅ Identify and exploit JavaScript vulnerabilities

### TypeScript
- ✅ Write type-safe Node.js applications
- ✅ Use advanced TypeScript features (generics, mapped types, conditional types)
- ✅ Design type-safe APIs and SDKs
- ✅ Apply design patterns with TypeScript

### Security
- ✅ Identify XSS, prototype pollution, injection vulnerabilities
- ✅ Perform security code reviews of JS/TS codebases
- ✅ Build security scanning tools
- ✅ Understand type safety limitations

### Bonus Skills
- ✅ Read and audit modern web app codebases (React/Next.js)
- ✅ Work with LLM SDKs in TypeScript (LangChain, Vercel AI)
- ✅ Build and publish npm packages

-----

## Resources Summary

### Essential (FREE)
- Eloquent JavaScript (FREE online)
- TypeScript Handbook (FREE official docs)
- JavaScript30 (FREE challenges)
- OWASP resources (FREE)

### Books You Own
- Web Development with Node and Express (Brown)
- You Don't Know JS (Simpson)
- Node.js: The Comprehensive Guide (Springer)
- Eloquent JavaScript (Haverbeke)

### Optional Purchases
- Programming TypeScript (Cherny) - ~$40 ✅ Recommended
- Node.js Design Patterns, 3rd ed - ~$45 ⚠️ Optional
- Execute Program subscription - $20/mo ⚠️ Optional

**Total Additional Cost: $0-85**
- Minimum: $0 (all free resources)
- Recommended: $40 (Programming TypeScript)
- Maximum: $85 (both books)

-----

## Weekly Study Tips

**For JavaScript (Weeks 47-52):**
- Do ALL exercises in Eloquent JavaScript
- Type code examples yourself (don't copy-paste)
- Build the projects fully - they're excellent

**For TypeScript (Weeks 53-58):**
- Fight the urge to use `any` everywhere
- Read compiler errors carefully - they teach you
- Enable `strict: true` from day one

**For Security (Weeks 63-66):**
- Actually exploit vulnerable apps (DVNA, NodeGoat)
- Document your findings thoroughly
- Practice responsible disclosure if you find real bugs

-----

## Success Criteria

**You're ready for production work when:**
- ✅ Can build type-safe REST APIs in TypeScript
- ✅ Understand async/await and promises deeply
- ✅ Can perform security code reviews
- ✅ Identify common JS/TS vulnerabilities
- ✅ Built at least 3 complete projects
- ✅ Comfortable reading React/Next.js codebases
- ✅ Can work with LLM SDKs (LangChain, etc.)
