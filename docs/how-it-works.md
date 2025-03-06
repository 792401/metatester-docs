---
sidebar_position: 2
---

# How it works

1. Build and run the tests
2. For each test, Metatester intercepts the request and saves the original response
3. Next, it runs the test N times against all configured N faults, by modifying the original response each time; request is also directed to a proxy
3. If test assertions fail against the simulated fault, test is marked as passed, since it caught the fault; otherwise marked as failed
4. Everything is collected in a report