---
sidebar_position: 2
---

# How it works

For each test, Metatester intercepts the request and saves the original response.

Next, it runs the test N times against all configured N faults, by modifying the original response each time; request is also directed to a proxy.

If test assertions fail against the simulated fault, test is marked as passed, since it caught the fault; otherwise marked as failed.

Everything is collected in a report.