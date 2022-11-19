# Tekton pipeline - IBM Container Registry docker images Vulnerability Scanning with Trivy

Using Aquasec Trivy, this sample tekton pipeline does Vulnerability Scanning of the docker image available in the IBM Container Registry.

## Aquasec Trivy

Trivy GitHub doc
https://github.com/aquasecurity/trivy


DevSecOps using Aquasec Trivy
https://developer.ibm.com/recipes/tutorials/devsecops-using-aquasec-trivy/

## Environment

This script works well in the following environment.

- OpenShift Version 4.4.17
- OpenShift Pipelines Operator 1.0.1 provided by Red Hat

## Installation and Run

1. Update `2-secrets.yaml` line no `13` with your `IBM Container Registry API Key`
2. Update `4-pipeline.yaml` line no `13` with your `image name`.
3. Goto the `install` folder
4. Run the command `sh 01-install.sh`
5. Goto the `Pipelines > Pipelines` in the OCP web console and click on `Start`  on the appropriate Pipeline.
