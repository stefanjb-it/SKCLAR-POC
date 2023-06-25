# SKCLAR-POC

[![Clear Azure](https://github.com/stefanjb-it/SKCLAR-POC/actions/workflows/clear_manual_azurecli.yml/badge.svg?branch=main)](https://github.com/stefanjb-it/SKCLAR-POC/actions/workflows/clear_manual_azurecli.yml)

**Clear Azure Workflow:**
- runs on dispatch event --> Button press required
- uses the Clear.azcli file to access the rg
- deletes all resources in the configured rg
- deletion errors are ingored because of force delete

[![Manual Deploy](https://github.com/stefanjb-it/SKCLAR-POC/actions/workflows/deploy_manual_azurecli.yml/badge.svg)](https://github.com/stefanjb-it/SKCLAR-POC/actions/workflows/deploy_manual_azurecli.yml)

**Manual Azure Deployment Workflow:**
- runs on dispatch event --> Button press required
- uses all azcli files in azurecli branch without Clear.azcli
- creates all resources in configured rg
- error are send by mail and displayed in Actions and badge

[![Release Deploy](https://github.com/stefanjb-it/SKCLAR-POC/actions/workflows/deploy_release_azurecli.yml/badge.svg)](https://github.com/stefanjb-it/SKCLAR-POC/actions/workflows/deploy_release_azurecli.yml)

**Release Azure Deployment Workflow:**
- runs on release event in the azurecli branch
- uses all azcli files in azurecli branch without Clear.azcli
- creates all resources in configured rg
- error are send by mail and displayed in Actions and badge
