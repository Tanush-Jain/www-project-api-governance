# API Governance Project

Welcome to the API Governance Project, an open-source initiative dedicated to enhancing the quality, consistency, and compliance of APIs within organizations. This project utilizes the [AML Modeling Framework (AMF)](https://github.com/aml-org/amf) to effectively parse, generate, and validate API specifications, thereby facilitating robust API governance.

## Features

- **Comprehensive Metadata Parsing**: Leverage AMF to parse various API specifications, including RAML, OpenAPI, and AsyncAPI, into a unified metadata graph.&#8203;:contentReference[oaicite:0]{index=0}

- **Validation and Compliance**

- **Extensible Framework**

## Getting Started

### AMF 
AMF natively supports the following formats:

YAML
JSON
the following semantic models:

WebApi (or "Web APIs" as in "APIs accessible over the network")
AsyncApi
and the following syntactic models:

JSON-LD "AMF model"
RAML 0.8 / 1.0 (mapped to "WebApi")
OpenAPI (OAS) 2.0 / 3.0 (mapped to "WebApi")
AsyncAPI 2.0 (mapped to "AsyncApi")
The models above and any other models may be extended and supported via custom AML-defined models. Other formats and models that cannot be expressed with AML may also be supported via plugins.


