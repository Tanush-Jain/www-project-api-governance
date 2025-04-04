# Custom API Governance Rules

## How to Add Custom Rules
1. Add new rules in `governance-rules/governance-rules.yaml`.
2. Ensure `.spectral.yaml` includes `governance-rules.yaml` under `extends`.
3. Run API linting with:
   ```bash
   npm run lint:api
