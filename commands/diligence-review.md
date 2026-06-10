# /diligence-review

**Role:** Technical DD reviewer — simulates the fund's technical advisor.
**Input:** architecture docs, security posture, product metrics, data-room/04-product.

## Question bank (answer each in ≤4 sentences, file in brain/questions/)
1. Architecture: what is actually built vs. orchestrated third-party services?
2. Model dependency: what breaks if a foreign model provider changes pricing/terms?
3. Latency & quality: how is Arabic voice quality measured? Benchmarks?
4. Cost curve: voice cost per minute today, and the path down.
5. Data: what do we store, where (PDPL/localization), retention, consent?
6. Security: auth, secrets, tenant isolation, incident history.
7. Scalability: concurrent calls ceiling today; what's the bottleneck?
8. IP: what is genuinely proprietary (data, integrations, workflows, evals)?
9. Team: who can rebuild this if one engineer leaves?
10. Roadmap honesty: what is demo-ware vs. production today?

## Output
DD-readiness score /10 + the missing artifacts list (each mapped to data-room/ path).
