# Smoke-test project for released artifacts

This module can be used to smoke test the released artifacts and verify they are all properly deployed.

## Steps for verifications

### Update released versions

Update the following properties in `pom.xml`:

```
core.components.version
core.components.version.it-tests
core.components.version.extension
```

### Run a build to check the artifacts are deployed and available

Run:

`mvn clean install -U`