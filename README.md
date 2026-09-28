# 60-Day Modern Java Architecture & Enterprise AI Engineering Sprint

Targeted daily 30-minute architectural modules calibrated for a Senior/Staff Java Engineer (7+ YOE).

## Daily Progress & Interview Tracker

### Phase 1: Modern Java & JVM Architecture (Days 01–30)

| Day | Topic | Key Interview Question | Status |
|:---:|---|---|:---:|
| 01 | JVM Memory Internals & Modern GC (G1 vs ZGC) | How does ZGC achieve sub-millisecond pause times compared to G1, and when would you avoid it? | [ ] |
| 02 | Java Memory Model (JMM): Visibility & Memory Barriers | Why does `volatile` prevent instruction reordering, and how do acquire/release semantics work? | [ ] |
| 03 | Low-Level Concurrency: CAS, `VarHandle` & Atomic Primitives | How does lock-free synchronization via CAS differ from kernel-mediated mutexes under high contention? | [ ] |
| 04 | Modern Asynchronous Workflows: `CompletableFuture` Internals | How do you prevent thread starvation in common ForkJoinPool when chaining async I/O stages? | [ ] |
| 05 | Modern I/O: Off-Heap Memory, Direct Buffers & Zero-Copy | What is the performance trade-off of Direct ByteBuffers vs Heap ByteBuffers in high-throughput network I/O? | [ ] |
| 06 | Modern HTTP Engine: Java `HttpClient` & Reactive Streams | How does Java 11+ `HttpClient` handle multiplexing and backpressure without third-party libraries? | [ ] |
| 07 | Production JVM Diagnostics: JFR, JMC & Safepoint Profiling | How do safepoint bias and Time-To-Safepoint (TTSP) issues degrade p99 latencies in production? | [ ] |
| 08 | Modern Data Modeling: Records & Compact Constructors | How do Records guarantee shallow immutability and optimize serialization security vulnerabilities? | [ ] |
| 09 | Pattern Matching for `switch` & Record Deconstruction | How does type pattern matching in `switch` eliminate defensive casts and handle `null` safely? | [ ] |
| 10 | Domain Modeling: Sealed Hierarchies & Algebraic Types | How do sealed classes provide compile-time exhaustiveness, eliminating the Gang of Four Visitor Pattern? | [ ] |
| 11 | Sequenced Collections Framework (Java 21) | What architectural inconsistencies in `Collection` and `Map` did JEP 431 resolve? | [ ] |
| 12 | Stream Processing: Clean Code, Gatherers (JEP 461/473) | How do Stream Gatherers allow custom intermediate operations (windowing/folding) without state corruption? | [ ] |
| 13 | Strings & Text: String Templates, Text Blocks & UTF-8 | How do modern String templates prevent injection attacks (SQL/NoSQL) at compile time? | [ ] |
| 14 | Foreign Function & Memory (FFM) API vs Legacy JNI | How does the FFM API eliminate JNI overhead and memory leaks when invoking native C libraries? | [ ] |
| 15 | Project Loom: Virtual Threads Architecture & Carrier Pools | What are the internals of mounting/unmounting virtual threads to OS carrier threads during blocking calls? | [ ] |
| 16 | Loom Pitfalls: Thread Pinning & Diagnostics | What causes Virtual Thread pinning with `synchronized` blocks, and how do you detect it using JFR? | [ ] |
| 17 | Structured Concurrency (`StructuredTaskScope`) | How does Structured Concurrency prevent thread leaks and enforce subtask cancellation deadlines? | [ ] |
| 18 | Context Propagation: Scoped Values vs `ThreadLocal` | Why are Scoped Values superior to `ThreadLocal` in memory footprint and immutability under virtual threads? | [ ] |
| 19 | Loom Migration: HikariCP, JDBC & Semaphore Throttling | Why should you never pool Virtual Threads, and how do you size database pools when requests explode? | [ ] |
| 20 | Concurrency Benchmarks: Virtual Threads vs WebFlux | In what precise system design scenarios does Reactive Programming still outperform Loom? | [ ] |
| 21 | Architectural Checkpoint: Refactoring Legacy Services to Loom | What are the end-to-end steps to refactor a thread-per-request blocking service without breaking contracts? | [ ] |
| 22 | Spring Boot 3 Core: Jakarta EE & Reflection/Proxy Shifts | What breaking changes occur during Spring Boot 2.7 to 3.x migration regarding proxy mechanisms? | [ ] |
| 23 | Declarative Clients: Spring 6 `RestClient` & `@HttpExchange` | When would you choose synchronous `RestClient` over reactive `WebClient` in a Java 21+ deployment? | [ ] |
| 24 | Spring Boot 3 AOT Compilation & GraalVM Native Image | How does closed-world assumption in AOT compilation impact dynamic class loading and reflection? | [ ] |
| 25 | Unified Observability: Micrometer Observation API | How does the Observation API unify metrics, distributed tracing (W3C/Zipkin), and context logging? | [ ] |
| 26 | Production Resilience: Resilient Loom Microservice Adapters | How do circuit breakers and rate limiters integrate with unpooled Virtual Thread workers? | [ ] |
| 27 | Secure Stateless Microservices: OAuth2 / OIDC & RFC 7807 | How do you implement RFC 7807 Problem Details while keeping error boundaries strictly typed? | [ ] |
| 28 | Modern Integration Testing: Testcontainers & Dynamic Properties | How does `@DynamicPropertySource` isolate ephemeral container ports during integration tests? | [ ] |
| 29 | JVM Optimization: CDS, AppCDS & Project Leyden | How does Application Class Data Sharing (AppCDS) drastically cut container cold-start times? | [ ] |
| 30 | Phase 1 Capstone: High-Throughput Observable Microservice | How do you architect a Java 21 + Spring Boot 3 service handling 50k RPS with low p99 latency? | [ ] |