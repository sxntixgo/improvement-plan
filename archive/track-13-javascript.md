# Track 13: JavaScript/TypeScript

**Duration:** 14 weeks | **Hours/week:** 18 | **Priority:** MEDIUM
**Goal:** Full-stack JS/TS for security tooling and modern web applications

**Learning Path:** JavaScript Fundamentals -> TypeScript -> Security

**Weekly Schedule:**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

> **Compression Note:** This track is compressed from 20 weeks to 14 weeks. By this
> point in the plan you have completed Python (Track 3) and Go (Track 7), so you
> already understand variables, control flow, functions, data structures, error
> handling, modules, async patterns, and static typing. The JavaScript fundamentals
> phase in particular is cut in half because you are learning a third programming
> language, not your first. The focus shifts to what makes JavaScript *different*:
> prototypes, closures, `this`, the event loop, and the ecosystem. TypeScript
> advanced theory is also trimmed -- you already think in types from Go.

-----

## Why JavaScript -> TypeScript?

**TypeScript is essential for modern AI/ML tooling:**
- LangChain, Vercel AI SDK, and many LLM tools use TypeScript
- Modern web apps (React/Next.js) use TypeScript
- Better code reading with type definitions
- But you need JavaScript fundamentals first

**Learning Path:**
1. **Weeks 49-51:** Pure JavaScript (foundation, compressed)
2. **Weeks 52-56:** TypeScript for Node.js/Express
3. **Weeks 57-58:** Advanced TypeScript essentials
4. **Weeks 59-62:** Security in both JS and TS

-----

## Phase Overview

|Phase|Weeks|Focus                            |Primary Resource              |
|-----|-----|---------------------------------|------------------------------|
|1    |49-51|JavaScript Fundamentals          |Eloquent JavaScript           |
|2    |52-56|Node.js & Express with TypeScript|TypeScript Handbook + Brown   |
|3    |57-58|TypeScript Advanced Essentials   |TypeScript Handbook + Patterns|
|4    |59-62|Security Focus (JS & TS)         |Eloquent JS Ch 13-15, 18 + OWASP + Hands-on|

-----

## Resources

### Books You Already Own

|Book                                         |Phase|Type          |
|---------------------------------------------|-----|--------------|
|Eloquent JavaScript (Haverbeke)              |1    |Project-driven|
|Web Development with Node and Express (Brown)|2    |Project-driven|
|You Don't Know JS 1st edition (Simpson)      |1,4  |Deep dive     |
|Node.js: The Comprehensive Guide (Springer)  |2-4  |Reference     |
|JavaScript and jQuery (Jon Duckett)          |1    |Visual supplement (OPTIONAL)|

**Eloquent JavaScript, 4th Edition (Haverbeke) — You're reading 17 of 22 chapters.** Reading Part I (Language) in full + security-relevant browser chapters + Node.js. Skipping only project chapters and canvas.

|Chapter|Title                                      |What to Do                                              |
|-------|-------------------------------------------|---------------------------------------------------------|
|1      |Values, Types, and Operators               |⭐ READ (Week 49) — Speed run; focus on JS type coercion  |
|2      |Program Structure                          |⭐ READ (Week 49) — let/const/var, hoisting               |
|3      |Functions                                  |⭐ READ (Week 49) — CRITICAL: closures, arrow functions, scope|
|4      |Data Structures: Objects and Arrays        |⭐ READ (Week 49) — Destructuring, spread, array methods  |
|5      |Higher-Order Functions                     |⭐ READ (Week 49) — map/filter/reduce, functional patterns|
|6      |The Secret Life of Objects                 |⭐ READ (Week 50) — CRITICAL: prototypes, `this`, classes |
|7      |Project: A Robot                           |⭐ READ (Week 50) — Build simulation, practice JS idioms  |
|8      |Bugs and Errors                            |⭐ READ (Week 50) — JS exception handling, fast review    |
|9      |Regular Expressions                        |⭐ READ (Week 50) — JS regex methods + ReDoS security angle|
|10     |Modules                                    |⭐ READ (Week 51) — ES modules vs CommonJS, npm           |
|11     |Asynchronous Programming                   |⭐ READ (Week 51) — CRITICAL: event loop, promises, async/await|
|12     |Project: A Programming Language            |⭐ READ (Week 51) — AST concepts for security tooling later|
|13     |JavaScript and the Browser                 |⭐ READ (Week 59) — Browser execution model, security context|
|14     |The Document Object Model                  |⭐ READ (Week 59) — CRITICAL for DOM-based XSS attacks    |
|15     |Handling Events                            |⭐ READ (Week 59) — Event handlers are XSS sinks          |
|16     |Project: A Platform Game                   |SKIP — Browser game project, not security-relevant        |
|17     |Drawing on Canvas                          |SKIP — Canvas API, not relevant                           |
|18     |HTTP and Forms                             |⭐ READ (Week 59) — Browser HTTP, CSRF, form-based attacks|
|19     |Project: A Pixel Art Editor                |SKIP — Browser project                                    |
|20     |Node.js                                    |⭐ READ (Week 52) — Node.js foundation before Express book|
|21     |Project: Skill-Sharing Website             |SKIP — Covered by Express project work                    |
|22     |JavaScript and Performance                 |SKIP — Skim if curious; not essential for your path       |

**Web Development with Node and Express, 2nd Edition (Brown) — You're reading 12 of 23 chapters.** Skipping email, SPA, static content, and maintenance chapters.

|Chapter|Title                                      |What to Do                                              |
|-------|-------------------------------------------|---------------------------------------------------------|
|1      |Introducing Express                        |⭐ READ (Week 52) — Framework overview, fast              |
|2      |Getting Started with Node                  |⭐ READ (Week 52) — Node.js basics                        |
|3      |Saving Time with Express                   |⭐ READ (Week 52) — Express scaffolding                   |
|4      |Tidying Up                                 |⭐ READ (Week 52) — Project structure                     |
|5      |Quality Assurance                          |⭐ READ (Week 52) — Testing with Jest + TypeScript        |
|6      |The Request and Response Objects           |⭐ READ (Week 52) — Request/response types                |
|7      |Templating with Handlebars                 |⭐ READ (Week 53) — Type-safe view rendering              |
|8      |Form Handling                              |⭐ READ (Week 53) — Request body typing, validation       |
|9      |Cookies and Sessions                       |⭐ READ (Week 53) — Type-safe session data                |
|10     |Middleware                                 |⭐ READ (Week 53) — CRITICAL: middleware chains, error handling|
|11     |Sending Email                              |SKIP — Email sending, not relevant to security tooling    |
|12     |Production Concerns                        |SKIP — Covered in Week 56 deployment section              |
|13     |Persistence                                |⭐ READ (Week 54) — Database integration with TypeScript  |
|14     |Routing                                    |⭐ READ (Week 54) — Type-safe route handlers              |
|15     |REST APIs and JSON                         |SKIP — You build REST APIs hands-on in Weeks 54-56        |
|16     |Single-Page Applications                   |SKIP — SPA concepts, not your focus                       |
|17     |Static Content                             |SKIP — Static file serving, trivial                       |
|18     |Security                                   |⭐ READ (Week 55) — bcrypt, JWT, HTTPS, security headers  |
|19     |Integrating with Third-Party APIs          |⭐ READ (Week 55) — OAuth, type-safe API clients          |
|20     |Debugging                                  |SKIP — Debugging basics, you know this                    |
|21     |Going Live                                 |SKIP — Deployment covered in Week 56 hands-on             |
|22     |Maintenance                                |SKIP — Long-term maintenance, not relevant yet            |
|23     |Additional Resources                       |SKIP — Resource list, not a chapter                        |

**You Don't Know JS, 1st Edition (Simpson)** — Use as supplement only. Read scope/closures chapters alongside Eloquent JS Week 49 if you need deeper explanations. Not a primary read.

**Node.js: The Comprehensive Guide (Springer)** — Reference only. Look up specific topics as needed during Weeks 52-56. Not read cover-to-cover.

**Note on Duckett book:**
- **Use ONLY as visual supplement** during Week 49 (JavaScript basics)
- Good for: Visual explanations, diagrams, color-coded examples when Eloquent JavaScript is confusing
- Skip entirely: All jQuery sections (second half of book) -- jQuery is outdated
- Don't replace: This is NOT a substitute for Eloquent JavaScript
- **How to use:** If a concept (closures, prototypes, etc.) isn't clicking in Eloquent JavaScript, flip to Duckett for the visual explanation, then return to Eloquent JavaScript

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
|Programming TypeScript (Cherny)|~$40   |Yes - very practical, examples   |
|Node.js Design Patterns (3rd ed)|~$45  |Yes - includes TypeScript        |
|Execute Program subscription   |$20/mo |Optional - excellent but pricey  |

**Recommended:** Stick with FREE resources (TypeScript Handbook is excellent). Only buy *Programming TypeScript* if you want a structured reference.

-----

## Phase 1: JavaScript Fundamentals (Weeks 49-51)

**Goal:** Master JavaScript-specific concepts quickly, building on your Python and Go foundation
**Primary Resource:** Eloquent JavaScript, 4th Edition (FREE at eloquentjavascript.net)

> **Why only 3 weeks?** You already know how to program. You know variables,
> loops, functions, data structures, error handling, and modules from Python
> and Go. These 3 weeks focus exclusively on what makes JavaScript *different*:
> prototypes, closures, `this` binding, type coercion, the event loop, and
> the async model. Skim what you know; dig deep on what is new.

### Week 49: JS Basics, Data Structures & Higher-Order Functions

**Eloquent JavaScript: Chapters 1-5 (18 hours)**

*Combines original Weeks 47-48. Chapters 1-2 will be fast review since you know programming. Spend the bulk of your time on Chapters 3-5.*

**Monday (3 hours): Chapters 1-2 (Speed Run)**
- Chapter 1: Values, Types, and Operators (1 hour)
  - Focus on what differs from Python/Go: type coercion, `==` vs `===`, `null` vs `undefined`
  - Skim: basic operators, strings, booleans (you know this)
- Chapter 2: Program Structure (2 hours)
  - `let` vs `const` vs `var` (understand hoisting -- new concept)
  - Control flow (skim -- same as every language)
  - Exercises: FizzBuzz, chessboard (fast -- you've done these)

**Tuesday-Wednesday (6 hours): Chapter 3 - Functions (JS-Specific Deep Dive)**
- Function declarations vs expressions vs arrow functions (2 hours)
  - This is NOT like Python `def` or Go `func` -- three syntaxes with different behaviors
- **Closures** (2 hours) -- THE critical JS concept
  - Lexical scoping
  - Closure over variables (not values)
  - Common closure pitfalls (loop variable capture)
- Scope and recursion (2 hours)
  - Scope chain
  - YDKJS 1st ed: Scope overview (supplement)
- Exercises: Minimum, recursion, bean counting

**Thursday-Friday (6 hours): Chapter 4 - Data Structures**
- Arrays and objects (2 hours)
  - Destructuring (new syntax vs Python unpacking)
  - Spread operator
  - Mutability model (different from Go)
- Array methods: map, filter, reduce, find, some, every (3 hours)
  - These are your bread and butter in JS -- drill them
- JSON, rest parameters (1 hour)
- Exercises: Sum of range, reversing arrays, deep comparison

**Weekend (3 hours): Chapter 5 - Higher-Order Functions**
- Abstraction with functions, passing functions as values (1 hour)
  - Familiar from Python, but JS idioms differ
- Array methods deep dive with exercises (2 hours)
  - Exercises: Flattening, your own loop, everything

-----

### Week 50: Objects, Prototypes, Error Handling & Regex

**Eloquent JavaScript: Chapters 6-9 (18 hours)**

*Combines original Weeks 49-50. Prototypes and the object model are the most important JS-specific concepts here. Error handling and regex will be fast review.*

**Monday-Tuesday (6 hours): Chapter 6 - The Secret Life of Objects**
- **Prototypes** (3 hours) -- THIS is the big JS-specific concept
  - Prototype chain (completely different from Python classes or Go interfaces)
  - `__proto__` vs `.prototype`
  - `Object.create`, `Object.getPrototypeOf`
- Classes (ES6 syntax) (2 hours)
  - Syntactic sugar over prototypes -- understand what's underneath
  - Getters, setters, statics
  - `this` binding rules (4 rules -- unique to JS)
- Exercises: A vector type, groups, iterable groups (1 hour)

**Wednesday (3 hours): Chapter 7 - Project: A Robot**
- Build delivery robot simulation (3 hours)
  - Graph theory, pathfinding -- focus on the JS idioms used
  - **Deliverable:** Working robot simulation (GitHub)

**Thursday (3 hours): Chapter 8 - Bugs and Errors (Fast)**
- Skim: debugging, strict mode (you know this from Python/Go) (1 hour)
- Focus: Exceptions in JS -- `try/catch/finally`, error propagation (1 hour)
  - Compare with Go's explicit error returns and Python's exception model
- Exercises: Retry, the locked box (1 hour)

**Friday-Weekend (6 hours): Chapter 9 - Regular Expressions**
- Regex syntax (fast review -- same across languages) (2 hours)
- JS-specific regex methods: `test`, `exec`, `match`, `replace` (2 hours)
- **Security angle:** regex DOS attacks (ReDoS) (1 hour)
- Exercises: Regexp golf, quoting style, numbers again (1 hour)

-----

### Week 51: Modules, Async Programming & Language Project

**Eloquent JavaScript: Chapters 10-12 (18 hours)**

*Combines original Weeks 51-52. The async chapter is critical and gets the most time. The language project is compressed to a fast-build exercise.*

**Monday-Tuesday (6 hours): Chapter 10 - Modules**
- ES modules vs CommonJS (3 hours)
  - `import/export` vs `require/module.exports`
  - This is a JS ecosystem split you need to understand
  - Compare with Python imports and Go packages
- npm basics, packages, module design (2 hours)
- Exercise: A modular robot (1 hour)

**Wednesday-Friday (9 hours): Chapter 11 - Asynchronous Programming (CRITICAL)**
- **The event loop** (3 hours) -- THE concept that makes JS unique
  - Single-threaded, non-blocking I/O
  - Call stack, task queue, microtask queue
  - Namaste JavaScript: Event loop episodes (YouTube supplement)
  - Compare with Go's goroutines/channels and Python's asyncio
- Callbacks and callback hell (1 hour)
- **Promises** (3 hours)
  - `then`, `catch`, `finally`
  - Promise chaining
  - `Promise.all`, `Promise.race`, `Promise.allSettled`
  - Build your own `Promise.all`
- **Async/await** (2 hours)
  - Syntactic sugar over promises
  - Error handling with try/catch in async functions
  - Exercises: Tracking scalpel

**Weekend (3 hours): Chapter 12**
- Chapter 12: Project: A Programming Language (3 hours)
  - Build parser + evaluator for Egg language (abbreviated)
  - Focus on understanding AST concepts -- you will need these for security tooling later
  - You already built interpreters; focus on JS-specific implementation style

**Deliverable:** Working Egg interpreter (GitHub -- abbreviated version is fine)

-----

## Phase 2: Node.js & Express with TypeScript (Weeks 52-56)

**Goal:** Learn Node.js/Express directly in TypeScript
**Primary Resources:** TypeScript Handbook + Web Development with Node and Express (adapted to TS)

> **Compression note:** TypeScript basics are folded into the first week alongside
> Express setup. Coming from Go's static type system, TypeScript's type syntax
> will feel natural. The focus is on getting productive fast.

### Week 52: TypeScript Fundamentals + Node.js + Express Setup

**Monday (2 hours): Eloquent JavaScript Ch 20 - Node.js**
- Node.js architecture: event loop, non-blocking I/O, streams
- File system, HTTP module, npm ecosystem
- Read this BEFORE diving into Express — gives you the foundation the Express book builds on

**Tuesday-Wednesday (7 hours): TypeScript Basics + Node.js Setup**

*TypeScript basics are compressed because you already know static typing from Go. Focus on TS-specific features.*

**TypeScript Handbook (4 hours):**
- **The Basics** (1 hour)
  - Static type checking, types vs values, `tsc` compiler
  - Skim quickly -- you understand static types from Go
- **Everyday Types** (2 hours)
  - Primitives, arrays, tuples
  - Objects and interfaces (compare with Go interfaces -- structural typing in both!)
  - Union types, type aliases, literal types (new -- Go doesn't have these)
- **Narrowing** (1.5 hours)
  - `typeof` guards, truthiness narrowing, equality narrowing
  - The `in` operator, discriminated unions
- **Functions** (1.5 hours)
  - Function type expressions, call signatures
  - Optional/default parameters, function overloads

**Node.js Setup with TypeScript (3 hours):**
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

- Simple TypeScript Node.js CLI tool
- File system operations with proper types
- **Practice:** Convert 1-2 Phase 1 JS projects to TypeScript

**Thursday-Weekend (9 hours): Express with TypeScript**

**Web Development with Node and Express (Brown) - Chapters 1-6, adapted to TypeScript**

- Chapters 1-4: Express intro and setup (3 hours)
  - Skim concepts (you know web servers from Go)
  - Focus on Express-specific patterns and middleware model
- Chapter 5: Quality Assurance (2 hours)
  - Testing with Jest + TypeScript
  - Type-safe testing
- Chapter 6: Request and Response Objects (4 hours)
  - Request/response types
  - Type-safe middleware

```bash
npm install express
npm install -D @types/express
```

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

**Reference:** Node.js: The Comprehensive Guide (Springer) - Chapters on Node.js basics

-----

### Week 53: Templates, Forms & Middleware

**Web Development with Node and Express - Chapters 7-10**

**Monday-Wednesday (9 hours): Templating & Forms**
- Chapter 7: Templating with Handlebars (3 hours)
  - Type-safe view rendering
  - Typed context objects
- Chapter 8: Form Handling (3 hours)
  - Request body typing
  - Validation with Zod or Joi
- Chapter 9: Cookies and Sessions (3 hours)
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

### Week 54: Database Integration with TypeScript

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

### Week 55: Authentication & Sessions

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

### Week 56: Production, Deployment & TypeScript Intermediate Patterns

**Monday-Wednesday (9 hours): TypeScript Intermediate Patterns**

**TypeScript Handbook:**
- **More on Functions** (2 hours)
  - Generic functions
  - Function constraints
- **Object Types** (2 hours)
  - Optional properties, readonly properties
  - Index signatures, extending types
- **Type Manipulation** (3 hours)
  - Generics, keyof/typeof operators
  - Conditional types, mapped types
  - Template literal types
- **Classes** (2 hours)
  - Class members, member visibility
  - Generic classes

**Thursday-Weekend (9 hours): Deployment**
- Production build setup
- Environment variables with type safety
- Docker with TypeScript
- Deployment to Vercel/Railway/Fly.io
- **Project:** Deploy your Express + TypeScript API

**Deliverable:** Production-ready REST API with full type safety (GitHub + blog post)

-----

## Phase 3: TypeScript Advanced Essentials (Weeks 57-58)

**Goal:** Practical advanced TypeScript for security tooling -- not type theory for its own sake

> **Why only 2 weeks?** You already work in a statically typed language (Go). You
> do not need 4 weeks of deep type theory. These 2 weeks cover the advanced
> patterns you will actually use when building security tools: generics for
> reusable components, design patterns for architecture, Result types for error
> handling, and enough testing to ship with confidence. Everything else you can
> learn on-demand.

### Week 57: Advanced Types, Design Patterns & Testing

**Monday-Tuesday (6 hours): Advanced Type Features**

**TypeScript Handbook:**
- **Creating Types from Types** (3 hours)
  - Generics deep dive
  - Indexed access types
  - Conditional types (practical patterns only)
  - Mapped types (Partial, Required, Pick, Omit)
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
type Immutable<T> = {
  readonly [P in keyof T]: T[P];
};
```

- **Type Guards & Narrowing** (3 hours)
  - Custom type guards (`is` keyword)
  - Discriminated unions (critical pattern)
  - Never type and exhaustiveness checking

**Wednesday-Thursday (6 hours): Design Patterns in TypeScript**

*Pick the patterns most relevant to security tooling. Skip academic completionism.*

**Essential Patterns (from Refactoring Guru + TypeScript):**
- Factory Pattern (1 hour) -- for creating different scanner/tester types
- Strategy Pattern (1.5 hours) -- for swappable analysis algorithms
- Observer Pattern (1.5 hours) -- for event-driven scanning
- Dependency Injection (2 hours) -- for testable, modular architecture

**Each pattern:**
1. Understand the pattern
2. Implement in TypeScript with full types
3. Connect to a security tooling use case

**Friday-Weekend (6 hours): Testing & Error Handling**

**Jest + TypeScript (3 hours):**
```bash
npm install -D jest ts-jest @types/jest
npx ts-jest config:init
```

- Unit testing with type safety (1.5 hours)
- Mocking with types (1 hour)
- Integration testing basics (0.5 hours)

**Error Handling Patterns (3 hours):**

**Result Type Pattern (critical for security tools):**
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

- Custom error types and error hierarchies (1 hour)
- Result/Option pattern (compare with Go's error returns) (1 hour)
- Practical: Add error handling to Week 56 project (1 hour)

-----

### Week 58: Capstone -- LLM Security Testing Tool

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

**Apply patterns from Week 57:**
- Factory pattern for LLMProvider creation
- Strategy pattern for different analysis approaches
- Result type for all fallible operations
- Full test suite with Jest

**Deliverable:**
- GitHub repo with full TypeScript codebase
- Blog post: "Building a Type-Safe LLM Security Tool"
- Published npm package (optional)

-----

## Phase 4: Security Focus (Weeks 59-62)

**Goal:** Security vulnerabilities in JavaScript and TypeScript

### Week 59: JavaScript Security Fundamentals

**Monday-Tuesday (6 hours): Eloquent JavaScript Ch 13-15, 18 — Browser Security Foundations**

Read these chapters BEFORE studying XSS — you need to understand the DOM and event model to understand how XSS attacks work:
- **Ch 13: JavaScript and the Browser (1 hour)** — Browser execution model, same-origin policy, security sandbox
- **Ch 14: The Document Object Model (2 hours)** — CRITICAL: DOM tree, node manipulation, innerHTML — these are XSS attack surfaces
- **Ch 15: Handling Events (1.5 hours)** — Event handlers as XSS sinks, event propagation, input handling
- **Ch 18: HTTP and Forms (1.5 hours)** — Browser HTTP requests, form submissions, CSRF attack surface

**Wednesday-Friday (6 hours): OWASP Top 10 for JavaScript**

**Topics:**
- XSS (Cross-Site Scripting) (2 hours)
  - DOM-based XSS (now you understand the DOM from Ch 14)
  - Reflected XSS
  - Stored XSS
- Prototype Pollution (2 hours)
  - Understanding prototypes (you covered this in Week 50 -- now attack them)
  - Attack vectors
  - Defensive coding
- Injection attacks (2 hours)
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

### Week 60: TypeScript Security & Best Practices

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
  db.create(user); // Vulnerable
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
  db.create(result.data); // Type-safe and validated
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
- **Practice:** Security audit of Week 56 project (1 hour)

-----

### Week 61: Security Tools & Testing

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

### Week 62: Security Code Review & Final Project

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

## Claude Code Integration

Use Claude Code throughout this track to accelerate learning and reinforce concepts.

**Phase 1 -- JavaScript Fundamentals (Weeks 49-51):**
- Ask Claude Code to explain confusing Eloquent JavaScript exercises before looking at solutions
- Use `/review` on your robot simulation and Egg interpreter to get idiomatic JS feedback
- Ask Claude Code to generate additional closure/prototype/`this` quiz questions when you need more practice
- Have Claude Code explain event loop execution order for tricky async examples

**Phase 2 -- Node.js & Express with TypeScript (Weeks 52-56):**
- Use Claude Code to scaffold Express + TypeScript boilerplate with proper `tsconfig.json`
- Ask it to review your type definitions -- it will catch `any` leaks and suggest stricter types
- Use Claude Code to generate Prisma schemas from your API design, then review the output
- When stuck on TypeScript compiler errors, paste the error and ask Claude Code to explain and fix

**Phase 3 -- Advanced TypeScript (Weeks 57-58):**
- Ask Claude Code to generate type challenges (e.g., "write a type that extracts all string keys from a nested object")
- Use it to review your design pattern implementations for TypeScript best practices
- Have Claude Code critique your LLM Security Testing Tool architecture before you build it
- Use `/review` on your capstone code to catch type safety gaps

**Phase 4 -- Security (Weeks 59-62):**
- Ask Claude Code to generate intentionally vulnerable code snippets for you to audit
- Use it to review your Semgrep rules and ESLint plugins for completeness
- Paste open-source code snippets and ask Claude Code to identify security issues -- then compare with your own findings
- Have Claude Code review your security scanner's detection logic for false positives/negatives

**General patterns throughout the track:**
- After completing any project, run `/review` to get feedback before moving on
- Use Claude Code to convert JavaScript examples to TypeScript when the book only shows JS
- Ask Claude Code to compare JS/TS patterns with their Python and Go equivalents to deepen your cross-language understanding

-----

## Projects & Outputs

|Project                          |Week   |Output                               |Share    |
|---------------------------------|-------|-------------------------------------|---------|
|Robot Simulation (Eloquent JS)   |50     |Delivery robot in JavaScript         |GitHub   |
|Egg Programming Language         |51     |Interpreter in JavaScript (abbrev.)  |GitHub   |
|Type-safe REST API               |54-56  |Express + TypeScript + Prisma        |GitHub   |
|LLM Security Testing Tool        |58     |CLI tool in TypeScript               |GitHub + npm|
|Custom Semgrep Rule              |61     |Security detection rule              |GitHub   |
|JavaScript Security Scanner      |62     |AST-based security scanner           |GitHub   |
|JS/TS Security Cheatsheet        |59-62  |Personal reference doc               |Blog post|

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

**By the end of Track 13, you should be able to:**

### JavaScript
- Write modern JavaScript with ES6+ features
- Understand closures, prototypes, and the event loop
- Build full-stack applications with Node.js/Express
- Identify and exploit JavaScript vulnerabilities

### TypeScript
- Write type-safe Node.js applications
- Use advanced TypeScript features (generics, mapped types, conditional types)
- Design type-safe APIs and SDKs
- Apply design patterns with TypeScript

### Security
- Identify XSS, prototype pollution, injection vulnerabilities
- Perform security code reviews of JS/TS codebases
- Build security scanning tools
- Understand type safety limitations

### Bonus Skills
- Read and audit modern web app codebases (React/Next.js)
- Work with LLM SDKs in TypeScript (LangChain, Vercel AI)
- Build and publish npm packages

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
- Programming TypeScript (Cherny) - ~$40 -- Recommended
- Node.js Design Patterns, 3rd ed - ~$45 -- Optional
- Execute Program subscription - $20/mo -- Optional

**Total Additional Cost: $0-85**
- Minimum: $0 (all free resources)
- Recommended: $40 (Programming TypeScript)
- Maximum: $85 (both books)

-----

## Weekly Study Tips

**For JavaScript (Weeks 49-51):**
- Do the Eloquent JavaScript exercises, but don't grind ones that test concepts you already know from Python/Go
- Spend extra time on closures, prototypes, `this`, and the event loop -- these are JS-unique
- Type code examples yourself (don't copy-paste)

**For TypeScript (Weeks 52-56):**
- Fight the urge to use `any` everywhere
- Read compiler errors carefully -- they teach you
- Enable `strict: true` from day one
- Compare TS patterns with Go equivalents to build intuition faster

**For Advanced TypeScript (Weeks 57-58):**
- Focus on patterns you will actually use in security tooling
- Skip deep type-level programming rabbit holes -- you can learn those on-demand
- The capstone project matters more than type theory

**For Security (Weeks 59-62):**
- Actually exploit vulnerable apps (DVNA, NodeGoat)
- Document your findings thoroughly
- Practice responsible disclosure if you find real bugs

-----

## Success Criteria

**You're ready for production work when:**
- Can build type-safe REST APIs in TypeScript
- Understand async/await and promises deeply
- Can perform security code reviews
- Identify common JS/TS vulnerabilities
- Built at least 3 complete projects
- Comfortable reading React/Next.js codebases
- Can work with LLM SDKs (LangChain, etc.)
