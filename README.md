# CI/CD Pipeline for a Containerized Web Application

## Overview

This repository contains a CI/CD pipeline for building, testing, and deploying a containerized React application to a Kubernetes cluster. The pipeline is implemented using GitHub Actions.

## CI/CD Workflow

The pipeline consists of the following jobs:

*   **Test & Lint:** Performs unit testing and static code analysis.
*   **Build:** Creates a production build of the React application.
*   **Docker Build & Push:** Builds and pushes a Docker image to the GitHub Container Registry, including a vulnerability scan with Trivy.
*   **Deploy:** Updates the Kubernetes deployment with the new image tag upon pushes to the `main` branch.

## Workflow Triggers

*   **Push** to `main` or `develop`.
*   **Pull Request** to `main` or `develop`.

## Technology Stack

*   **CI/CD:** GitHub Actions
*   **Containerization:** Docker
*   **Orchestration:** Kubernetes
*   **Frontend:** React, TypeScript
*   **Security:** Trivy
