# 🛡️ DevSecure API

Une petite API Python (Flask) conçue avec une approche **DevSecOps** : sécurisée dès le développement, containerisée et livrée via une pipeline CI/CD automatisée.

![CI/CD](https://github.com/Daniween/ci-cd-secure/actions/workflows/ci.yml/badge.svg)
![Docker](https://img.shields.io/badge/Docker-ready-blue)
![Security](https://img.shields.io/badge/Security-Scanned-brightgreen)

---

## 🔧 Fonctionnalités

- ✅ **API Python légère** (Flask ou FastAPI)
- 🐳 **Dockerisation** complète
- ⚙️ **Pipeline CI/CD GitHub Actions**
  - Build & test de l’image Docker
  - Scan de sécurité :
    - [Trivy](https://github.com/aquasecurity/trivy) (vulnérabilités)
    - [Snyk](https://snyk.io/) (dépendances & container)
    - [GitLeaks](https://github.com/zricethezav/gitleaks) (secrets dans le code)
  - Push automatique vers [Docker Hub](https://hub.docker.com/)
- 🧾 Génération de rapport HTML de vulnérabilités

---

## 🚀 Lancer en local

### 1. Cloner le projet

```bash
git clone https://github.com/Daniween/ci-cd-secure.git
cd ci-cd-secure
docker build -t devsecure-api .
docker run -p 3000:3000 devsecure-api
```
