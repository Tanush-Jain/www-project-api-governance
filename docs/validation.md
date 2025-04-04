# API Validation Rules in AMF

AMF (AML Modeling Framework) enforces strict validation rules to ensure API specifications comply with industry standards. Below are key validation checks for different formats:

## 🚀 RAML Validation Rules
| Rule | Description | ❌ Invalid Example | ✅ Valid Example |
|------|------------|----------------------|--------------------|
| Missing Base URI | The `baseUri` field is required in RAML. | `baseUri: ~` (empty) | `baseUri: "https://api.example.com"` |
| Invalid Data Type | Properties must have correct types. | `type: integer` (for string) | `type: string` |

## 🚀 OpenAPI Validation Rules
| Rule | Description | ❌ Invalid Example | ✅ Valid Example |
|------|------------|----------------------|--------------------|
| Missing Info Object | The `info` object is required in OpenAPI. | No `info` block | `info: {title: 'API', version: '1.0'}` |
| Invalid Path Parameter | Path params must be defined in `parameters`. | `{ "get": { "operationId": "getUser" }}` | `{ "parameters": [{ "name": "userId", "in": "path", "required": true }]}` |

## 🚀 AsyncAPI Validation Rules
| Rule | Description | ❌ Invalid Example | ✅ Valid Example |
|------|------------|----------------------|--------------------|
| Missing AsyncAPI Version | `asyncapi` field is mandatory. | `asyncapi: ~` | `asyncapi: "2.0.0"` |
| Invalid Channel Binding | Bindings must be properly structured. | `{ "bindings": { "http": { "type": "invalid" }}}` | `{ "bindings": { "http": { "type": "request" }}}` |

### 📌 Why This Matters?
- Ensures **API compliance with industry standards**.
- Helps developers **quickly debug validation issues**.
- Improves **overall API governance & documentation clarity**.

