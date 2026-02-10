# Mouaad Idoufkir (NZ4) — معاذ ادافقير

**Staff Software Engineer · Generative AI & Systems Researcher**
GitHub: **mouuuuaad**
Website: [https://github.com/mouuuuaad](https://github.com/mouuuuaad)
LinkedIn: [https://www.linkedin.com/in/mouaad-idoufkir](https://www.linkedin.com/in/mouaad-idoufkir)

---

## Profile

I am a Staff Software Engineer working at the intersection of **systems engineering, programming languages, and Generative AI**. My focus is on building software that is not only fast and scalable, but also conceptually clean and architecturally sound.

I spend most of my time designing **low-level systems**—compilers, runtimes, and high‑performance backends—where correctness, predictability, and long‑term maintainability matter more than short‑term convenience. I care deeply about understanding *how things work under the hood* and making design decisions explicit rather than implicit.

My core technical background includes **Rust, Go, Python, and Node.js**, with hands‑on experience across compiler construction, distributed systems, and production AI infrastructure.

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

## System-Level Architecture (High-Level)

ARNm is built as a **layered systems architecture**, intentionally designed to make responsibilities clear and behavior predictable. Rather than relying on hidden runtime magic, the language follows a *compiler–runtime co-design* approach where each layer has a well-defined role.

### Architectural Layers

**1. Language Semantics Layer**
Defines the programming model itself. The actor abstraction enforces isolated state, explicit communication, and a clear lifecycle for concurrent entities. Shared mutable memory is disallowed by design.

**2. Static Analysis & Type System Layer**
Responsible for enforcing correctness before execution. The type system and semantic checks aim to eliminate entire classes of errors early, especially those related to concurrency and invalid state transitions.

**3. Compiler Core (arnmc)**
Transforms source code into machine code through a traditional but explicit pipeline: parsing, semantic analysis, SSA-based IR construction, optimization, and architecture-aware code generation targeting x86_64. The goal is transparency rather than abstraction leakage.

**4. Runtime System (libarnm)**
Provides execution support without becoming a virtual machine. Actors are lightweight execution contexts scheduled in user space, communicating through mailboxes with minimal synchronization overhead.

**5. Execution & OS Interface**
A minimal C/assembly entry layer initializes the runtime and interfaces with the operating system. POSIX threads are used strictly as worker resources, not as a programming abstraction.

---

### Concurrency & Execution Model

ARNm employs a **many-actor / few-thread** model:

* Millions of actors mapped onto a small number of worker threads
* Central scheduler performs load balancing and wake-up signaling
* Actors execute in isolation and communicate strictly via messages

This model achieves scalability comparable to Erlang-style systems while preserving low-level performance characteristics.

---

### Design Principles

* **Isolation by construction**: Actors cannot share memory
* **Predictability over magic**: No hidden runtime behavior
* **Static guarantees before execution**
* **Runtime minimalism**: Everything not required is removed

ARNm intentionally avoids heavyweight abstractions (GC-heavy VMs, reflection, dynamic dispatch) in favor of explicit, analyzable system behavior.

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
