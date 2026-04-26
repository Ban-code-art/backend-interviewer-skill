# Backend Interview Question Bank

Use this bank to select adaptive questions based on user project.
Prefer project-grounded variants over abstract textbook questions.

## Round 1: Project Deep Dive

1. Give a 2-minute project overview: business value, architecture, and your ownership.
2. Which module was most complex, and why?
3. Describe one major incident you handled end-to-end.
4. What trade-off did you make under delivery pressure?
5. Which decision would you change if rebuilding today?

Follow-ups:
- What metric proved the improvement?
- What alternatives were rejected and why?
- What was the rollback plan?

## Round 2: Architecture and System Design

1. Draw the request path from ingress to storage, and identify bottlenecks.
2. Why microservices (or why not)? Discuss boundaries and coupling.
3. How do you handle service discovery, config, and failure isolation?
4. How do you ensure idempotency in write APIs?
5. Design a high-throughput order API with consistency requirements.

Follow-ups:
- CAP and consistency model for each critical operation
- Retry storms and cascading failure controls
- Backward compatibility and versioning strategy

## Round 3: Performance, Concurrency, Reliability

1. Where did latency come from and how did you profile it?
2. How did you optimize database hot paths and indexing?
3. Explain one concurrency bug (deadlock/race/oversell) and fix.
4. How do you design caching strategy and invalidation rules?
5. What is your approach to flow control, rate limiting, and graceful degradation?

Follow-ups:
- p95/p99 impact before and after
- Throughput vs consistency trade-off
- Thread pool, connection pool, and queue tuning rationale

## Round 4: Security, Deployment, Operations

1. How do you implement authN/authZ in backend services?
2. How do you prevent common vulnerabilities (SQL injection, SSRF, deserialization)?
3. Explain your CI/CD strategy, canary, and rollback guardrails.
4. How do you build observability: logs, metrics, traces, alerts?
5. Describe one on-call incident response timeline and lessons learned.

Follow-ups:
- Secret management and rotation
- Data encryption at rest/in transit
- Change failure rate and MTTR improvements

## Stack-Specific Probes

## Java / Spring Boot

1. How do you tune JVM for latency-sensitive services?
2. Explain Spring transaction boundaries and propagation choices.
3. How do you prevent N+1 query and ORM performance pitfalls?
4. How do you design resilient Feign/RestTemplate/WebClient calls?

## Go

1. Explain goroutine leak scenarios you encountered and detection method.
2. How did you choose channel vs mutex in a real module?
3. How do you control GC and memory growth in high-QPS services?
4. How do you structure context cancellation and timeout propagation?

## Database

1. How do you choose between strong consistency and eventual consistency?
2. Explain one schema/index evolution with zero downtime.
3. How do you handle distributed transaction requirements?
4. What was your read/write split strategy and risk?

## Microservices and Distributed Systems

1. How do you design bounded contexts and avoid chatty RPC?
2. How do you handle duplicate messages and exactly-once expectations?
3. Which circuit breaking and bulkhead patterns did you use?
4. How do you manage cross-service observability and root-cause analysis?

