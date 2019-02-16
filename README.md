# circleci-orb-job-expiration
CircleCI Orb to set job expiration 

https://circleci.com/orbs/registry/orb/azihsoyn/job-expiration

# Usage

Example config:

```yaml
version: 2.1

orbs:
  expiration: azihsoyn/job-expiration@0.1.0

jobs:
  build:
    docker:
      - image: <docker image>
    steps:
      - expiration/set:
          ttl: 600
      - expiration/check
```
