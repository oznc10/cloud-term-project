# Kampüs Kayıp Eşya — Multi-Cloud Lost & Found

A small campus lost-and-found web app built on **Azure + AWS** for the Cloud Computing term project.
Students sign in with Microsoft Entra ID, post found items with a photo, and browse or claim items.
Uploading a photo triggers a serverless function that generates a thumbnail.

> Status: work in progress

## Architecture
_Diagram will be added to `docs/`._

| Component | Cloud | Service | Why |
|---|---|---|---|
| Web interface | Azure | Static Web Apps | TBD |
| Backend API | Azure | Azure Functions | TBD |
| Database | Azure | Cosmos DB (free tier) | TBD |
| Authentication | Azure | Microsoft Entra ID | TBD |
| Secrets | Azure | Key Vault | TBD |
| Object storage | AWS | S3 (private bucket) | TBD |
| Event-driven function | AWS | Lambda (S3 upload trigger) | TBD |
| Analytics | Google | Google Analytics 4 | TBD |

Regions: Azure `swedencentral`, AWS `eu-north-1` (Stockholm).

## Repository layout
````
infra/bootstrap/   Terraform remote state backends
infra/azure/       Terraform stack for Azure
infra/aws/         Terraform stack for AWS
api/               Backend API (Azure Functions)
lambda/thumbnail/  S3-triggered thumbnail function (AWS Lambda)
frontend/          Browser front end
docs/              Architecture diagram and screenshots
.github/workflows/ CI/CD pipelines
````

## How to deploy
_TBD_

## Resources created manually
_TBD — every resource not created by Terraform will be listed and justified here._

## Cost
- Budget alerts: USD 5 on both Azure and AWS accounts.
- Estimate: _TBD_
- Actual cost screenshot: _TBD_

## Demo video
_TBD_

## Contribution
Solo project — all work by Ömer Özenç.
