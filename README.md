Perfect 👍 — here’s a polished version of your whole section, formatted so your team can drop it straight into your documentation:

---

# Billing

## Release Process

| Environment | Deployment Method                  | Instructions                                                                       |
| ----------- | ---------------------------------- | ---------------------------------------------------------------------------------- |
| **Dev**     | Deploy workflow dispatch           | Visit the [deploy workflow](deploy-workflow) and trigger with the desired options. |
| **Stage**   | Deploy workflow dispatch           | Visit the [deploy workflow](deploy-workflow) and trigger with the desired options. |
| **Prod**    | Release workflow dispatch (by tag) | Visit the [release workflow](release-workflow) and trigger with the relevant tag.  |

### Progessing to prod without stage deployment

If you need to deploy new changes to **Prod** without first deploying to **Stage**, select **Dev** as the `source_environment` in the Release workflow dispatch.

> **Note:** Selecting this option will skip the Stage deployment, and your changes will be deployed directly from Dev to Prod.

---

⚡ Do you want me to also add a **warning callout** (like “⚠️ Not recommended for normal releases”) to make it clear this should be used carefully?