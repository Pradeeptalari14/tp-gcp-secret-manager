# GCP Secret Manager Studio

This repository contains the target configuration and SRE runtime files compiled by the **GCP Secret Manager Studio** dashboard module.

## 🚀 Description
Store and manage API keys and keys versions on Google Cloud. Generate secret replication configurations, access permission maps, and programmatic retrieval SDKs.

## 🛠️ Specification Matrix
- **Primary Configuration File**: `/infra/secrets/secret_config.tf`
- **Execution Command**: `terraform init && terraform apply -auto-approve`
- **Validation Command**: `terraform show`

## 📋 How to Run & Validate

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pradeeptalari14/tp-gcp-secret-manager.git
   cd tp-gcp-secret-manager
   ```

2. **Run Execution Target:**
   ```bash
   terraform init && terraform apply -auto-approve
   ```

3. **Verify Runtime Stability:**
   ```bash
   terraform show
   ```

## 🔐 Security & Best Practices
* **Secret Isolation**: Use organization-level secrets (or SSM parameter hooks) rather than hardcoded environment variables inside files.
* **Pull Request Lifecycles**: Protect default branch merges with validation checks before merging code changes.
