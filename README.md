# Mouaad Idoufkir (NZ4) — معاذ ادافقير

**Staff Software Engineer · Generative AI & Systems Researcher**
GitHub: **mouuuuaad**
Website: [https://github.com/mouuuuaad](https://github.com/mouuuuaad)
LinkedIn: [https://www.linkedin.com/in/mouaad-idoufkir](https://www.linkedin.com/in/mouaad-idoufkir)

---

## Profile

I am a Staff Software Engineer focused on the design and implementation of **production-grade Generative AI systems** and **high-performance backend architectures**. My work spans programming language design, distributed systems, and applied AI research, with a strong emphasis on correctness, scalability, and performance.

Core expertise includes **Rust, Go, Python, Node.js**, low-level systems engineering, and compiler/runtime development.

---

## Links & Profiles

* GitHub: [https://github.com/mouuuuaad](https://github.com/mouuuuaad)
* ARNm Repository: [https://github.com/mouuuuaad/ARNm-Programming-Language](https://github.com/mouuuuaad/ARNm-Programming-Language)
* Mathematics Library (Go): [https://github.com/mouuuuaad/maths-with-golang](https://github.com/mouuuuaad/maths-with-golang)
* LinkedIn: [https://www.linkedin.com/in/mouaad-idoufkir](https://www.linkedin.com/in/mouaad-idoufkir)

---

## Current Research Project

### ARNm Programming Language

**Repository**: [https://github.com/mouuuuaad/ARNm-Programming-Language](https://github.com/mouuuuaad/ARNm-Programming-Language)
*A high-performance, actor-based programming language for massive concurrency.*

ARNm is a **statically typed, compiled systems language** designed from first principles to support scalable concurrency. It combines the **actor model** (inspired by Erlang) with **low-level performance characteristics** comparable to C and modern systems languages.

**Research Objectives**

* Formalize a lightweight actor model with strict memory isolation
* Achieve near–zero-cost abstractions through direct x86_64 code generation
* Design a runtime scheduler capable of supporting millions of concurrent actors
* Explore compiler–runtime co-design for safety and performance

**Key Properties**

* Native actor-based concurrency with message passing
* Static typing with compile-time guarantees
* Optimized SSA-based backend emitting x86_64 assembly
* User-space scheduler and mailbox-driven runtime

---

## Language Architecture (Summary)

**Compiler Pipeline**

* Lexing → Parsing → Semantic Analysis (Typed AST)
* SSA-based Intermediate Representation
* Optimization and direct x86_64 assembly generation

**Runtime System**

* User-space scheduler managing lightweight actors
* Worker-thread execution model
* Message queues (mailboxes) for inter-actor communication
* Minimal runtime with explicit initialization via `crt0`

This design enables predictable performance while preserving fault isolation and concurrency safety.

---

## Selected Software Contributions

### Pure Golang Mathematical Library

**Repository**: [https://github.com/mouuuuaad/maths-with-golang](https://github.com/mouuuuaad/maths-with-golang)
*A comprehensive, dependency-free mathematical systems library.*

* 15 mathematical modules
* 124 in-depth chapters
* Covers calculus, linear algebra, probability, optimization, graph theory, and differential equations
* All implementations written in **pure Go**, with production-grade correctness and test coverage

The project emphasizes algorithmic clarity, numerical stability, and educational rigor.

---

## Technical Competencies

**Programming Languages**
Rust · Go · Python · TypeScript · JavaScript

**Systems & Backend**
Compilers · Runtimes · Distributed Systems · Microservices · High-performance APIs

**AI & Machine Learning**
Generative AI · Deep Learning · NLP · Computer Vision · Model Deployment

**Infrastructure**
Docker · Kubernetes · Linux · Git · Cloud-native architectures

---

## Research & Engineering Interests

* Programming language design
* Actor models and concurrency theory
* Compiler optimization and IR design
* Runtime systems and schedulers
* Generative AI systems in production
* Mathematical foundations of computation

---

## Professional Philosophy

I approach software engineering as an applied research discipline: **clarity before cleverness, correctness before scale, and architecture before tooling**. My work aims to bridge theory and production, building systems that are both intellectually rigorous and operationally robust.

---

**Mouaad Idoufkir**
Staff Software Engineer · Generative AI & Systems
