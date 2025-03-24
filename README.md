# DevSecure API

Une petite API Python avec un pipeline CI/CD sécurisé.

## 🔧 Fonctionnalités :

- Dockerisation
- Pipeline GitHub Actions
- Scans de sécurité (Trivy, GitLeaks)
- Push auto sur Docker Hub

## 🚀 Lancer en local

```bash
docker build -t devsecure-api .
docker run -p 3000:3000 devsecure-api
```
