# Proof of Concept: Snyk Security Scanners

This sample repository is used to explore and test the snyk scanner options.

We created this mono-repo to simulate a typical work package, with:
 - some [configuration](./config) files (eg: dev / prod K8S manifests)
 - a [simple REST api](./packages/api) (packaged as container)
 - we deploy the app as a [helm chart](./helm/sample) to Kubernetes.

## Happy flow

This represents the "happy flow", where all resources are version controlled in git.

Unfortunately, this is not a very acurate real work example, as some of these file
(eg: `./dist/**`) is not typiucally version controlled.