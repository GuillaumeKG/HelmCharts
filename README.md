# HelmCharts
Contains HELM chart sources







## Deploying an application

Requirements
- Run as non root user
- Don't write on image filesystem (only mounted volume)
- Define request/limits
- Define liveness probe
- Define readiness probe (at least test that ssopv2 is responding)


Questions:
- Need for temporary volume?
- Need for config file?
- Need to access to: ssopv2? keysecure? smtp? other?
- Need for calling other BFOAs?
- How many replica needed in normal circumstances? Autoscaling? min/max?
-

Step:
- Run load testing to validate request/limits (Arnaud)