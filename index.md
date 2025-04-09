---

layout: col-sidebar
title: OWASP API Governance


---

# 🛡️ OWASP API Governance

A lightweight project for enforcing API governance using Spectral. It ensures your OpenAPI specifications follow best practices, consistent naming conventions, and organization-wide rules.

---

## 🚀 Features

- ✅ Lint OpenAPI 2.0 & 3.0 specs
- ✅ Custom governance rules with Spectral
- ✅ Naming conventions, summaries, tags, and more
- ✅ Optimized with compiled rulesets
- ✅ GitHub Actions support for CI linting

---


## 🧪 Linting Commands

Install dependencies:

```bash
npm install

Compile ruleset:
npm run lint:compile

Lint all API specs:
npm run lint:api

Lint a single API spec:
npx spectral lint -r compiled-ruleset.json specs/example-api.yaml

🤝 Contributing
Fork this repo

Create a new branch

Make changes

Run npm run lint:compile and npm run lint:api

Submit a PR 🎉

📜 License
Apache 2.0 License

🔗 Resources

OWASP API Security
Spectral: https://stoplight.io/open-source/spectral

