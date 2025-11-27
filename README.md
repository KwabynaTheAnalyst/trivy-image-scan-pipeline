# Container Image Scanning Pipeline with Trivy and GitHub Actions

This project builds a container image for a small Python application and scans it with Trivy during the CI process. The workflow generates a vulnerability report and enforces a security gate by failing the pipeline when High and Critical findings exceed a defined limit. An HTML report is uploaded as an artifact to support review and documentation.

/assets/images/devsecops/container_image-scanning_trivy.png

## Features

- Automated Docker image build on push or pull request  
- Trivy scan integrated into GitHub Actions  
- Threshold gate for High and Critical vulnerabilities  
- JSON output wrapped into a readable HTML report  
- Sample containerized application included for demonstration  

## Repository structure

```text
app/
  app.py
  requirements.txt
Dockerfile
.github/
  workflows/
    trivy-image-scan.yml
README.md
```




