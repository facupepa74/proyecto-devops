# 🚀 Proyecto DevOps: CI/CD Pipeline con Node.js, Docker, GitHub Actions y AWS EC2

Este repositorio contiene una aplicación web en **Node.js** y **Express**, empaquetada en un contenedor **Docker** y desplegada automáticamente en una instancia de **AWS EC2** mediante un pipeline continuo de **CI/CD con GitHub Actions**.

---

## 🛠️ Tecnologías Utilizadas

* **Backend:** Node.js, Express
* **Contenerización:** Docker, Docker Hub
* **CI/CD:** GitHub Actions
* **Cloud Infrastructure:** AWS EC2 (Ubuntu)
* **Seguridad:** SSH Keys, GitHub Secrets, Docker Personal Access Tokens (PAT)

---

## 🔄 Arquitectura del Pipeline (CI/CD)

El flujo de integración y despliegue continuo se dispara automáticamente ante cada `git push` a la rama principal (`main`):

```text
Local (VS Code) ──> Git Push ──> GitHub Actions ──> Build Docker Image ──> Docker Hub ──> SSH Deploy ──> AWS EC2