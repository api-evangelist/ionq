# IonQ (ionq)

IonQ (NYSE IONQ) is a College Park, Maryland-based public trapped-ion quantum computing company. IonQ designs, manufactures, and operates trapped-ion quantum computers (Aria, Forte, Forte Enterprise, Tempo, Harmony) and delivers them through the IonQ Quantum Cloud REST API, on-premises Forte Enterprise systems, and partner clouds (AWS Braket, Microsoft Azure Quantum, Google Cloud). The platform supports submission of QIS and native-gate circuits, multi-circuit and Quantum Function jobs, reserved Sessions, error mitigation, and organization-level usage and cost reporting. IonQ's quantum networking, security (QKD), sensing, and space-infrastructure businesses extend the trapped-ion core into a broader quantum systems portfolio.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/ionq/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/ionq/refs/heads/main/apis.yml)

## Scope

- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- Quantum Computing
- Trapped Ion
- QPU
- Aria
- Forte
- Tempo
- Quantum Cloud
- Cloud
- Hardware
- Public Company

## Timestamps

- **Created:** 2026-05-24T00:00:00.000Z
- **Modified:** 2026-05-24

## APIs

### IonQ Quantum Cloud API

REST API for submitting quantum circuits, managing jobs and sessions, inspecting backends and characterizations, and tracking cost and usage on the IonQ Quantum Cloud. Backends include the qpu.aria-1, qpu.aria-2, qpu.forte-1, qpu.forte-enterprise-1 trapped-ion QPUs and the IonQ noisy/ideal simulator (up to 29 qubits). Supports single-circuit, multi-circuit, native-gate, QAOA, and Quantum Function jobs. Authentication via Authorization header `apiKey $IONQ_API_KEY`.

- **Human URL:** [https://docs.ionq.com/api-reference/v0.4/introduction](https://docs.ionq.com/api-reference/v0.4/introduction)
- **Base URL:** `https://api.ionq.co/v0.4`

#### Tags

- Quantum Computing
- Trapped Ion
- QPU
- Jobs
- Sessions
- Backends
- Cloud

#### Properties

- [Documentation](https://docs.ionq.com/api-reference/v0.4/introduction)
- [Documentation](https://docs.ionq.com/guides/direct-api-submission)
- [OpenAPI](openapi/ionq-quantum-cloud-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ionq-quantum-cloud.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ionq-quantum-cloud.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/ionq-job-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/ionq-backend-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/ionq-session-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/ionq-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### IonQ Quantum Cloud API (v0.3 Legacy)

The previous-generation IonQ Quantum Cloud REST API (v0.3) for submitting and managing jobs, characterizations, backends, and reports. Superseded by v0.4 which adds Sessions, separated cost/results endpoints, and restructured characterizations. v0.3 remains supported for existing integrations.

- **Human URL:** [https://docs.ionq.com/api-reference/v0.3/introduction](https://docs.ionq.com/api-reference/v0.3/introduction)
- **Base URL:** `https://api.ionq.co/v0.3`

#### Tags

- Quantum Computing
- Trapped Ion
- QPU
- Legacy

#### Properties

- [Documentation](https://docs.ionq.com/api-reference/v0.3/introduction)
- [Documentation](https://docs.ionq.com/api-reference/v0.3/migrating-from-old-versions)
- [Documentation](https://docs.ionq.com/api-reference/v0.4/migration-from-v0.3)
- [Postman Collection](collections/ionq-quantum-cloud.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ionq-quantum-cloud.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://ionq.com)
- [Documentation](https://docs.ionq.com)
- [Documentation](https://docs.ionq.com/api-reference/v0.4/introduction)
- [Documentation](https://docs.ionq.com/api-reference/v0.3/introduction)
- [Portal](https://cloud.ionq.com)
- [Sign Up](https://cloud.ionq.com)
- [Documentation](https://docs.ionq.com/user-manual/introduction)
- [Glossary](https://docs.ionq.com/user-manual/glossary)
- [Authentication](https://docs.ionq.com/guides/managing-api-keys)
- [Authentication](https://docs.ionq.com/guides/connecting-saml-identity-providers)
- [Authentication](https://docs.ionq.com/guides/dotenv-project-api-keys)
- [Getting Started](https://docs.ionq.com/guides/direct-api-submission)
- [Getting Started](https://docs.ionq.com/guides/getting-started-with-native-gates)
- [Documentation](https://docs.ionq.com/guides/cloud-usage)
- [Documentation](https://docs.ionq.com/guides/error-mitigation-debiasing)
- [Documentation](https://docs.ionq.com/guides/qpu-submission-checklist)
- [Documentation](https://docs.ionq.com/guides/hosted-hybrid-service)
- [Documentation](https://docs.ionq.com/guides/simulation-with-noise-models)
- [Documentation](https://docs.ionq.com/guides/qaoa-solve-with-fire-opal)
- [Documentation](https://docs.ionq.com/user-manual/platform-systems)
- [Documentation](https://docs.ionq.com/user-manual/backends)
- [Documentation](https://docs.ionq.com/user-manual/jobs)
- [Documentation](https://docs.ionq.com/user-manual/projects)
- [Documentation](https://docs.ionq.com/user-manual/organizations)
- [Documentation](https://docs.ionq.com/user-manual/accounts)
- [Documentation](https://docs.ionq.com/partners/amazon-braket)
- [Versioning](https://docs.ionq.com/api-reference/v0.4/migration-from-v0.3)
- [Errors](https://docs.ionq.com/api-reference/v0.3/error-codes)
- [Status Page](https://status.ionq.co)
- [Support](https://support.ionq.com)
- [Support](mailto:support@ionq.com)
- [Contact](https://ionq.com/contact)
- [Blog](https://ionq.com/news)
- [Blog](https://ionq.com/posts)
- [Documentation](https://ionq.com/resources)
- [Portal](https://ionq.com/quantum-cloud)
- [Documentation](https://ionq.com/products)
- [Documentation](https://ionq.com/company)
- [Documentation](https://ionq.com/careers)
- [Documentation](https://investors.ionq.com)
- [Terms of Service](https://ionq.com/legal/terms-of-service)
- [Privacy Policy](https://ionq.com/legal/privacy-policy)
- [Documentation](https://ionq.com/legal)
- [GitHub Organization](https://github.com/ionq)
- [SDK](https://github.com/ionq/ionq-core-python)
- [SDK](https://pypi.org/project/ionq-core/)
- [SDK](https://github.com/ionq/blqs)
- [Tool](https://github.com/ionq/pyGSTi)
- [Tool](https://github.com/ionq/qrmi)
- [Tool](https://github.com/ionq/torchquantum-dist)
- [Tool](https://github.com/ionq/QC-App-Oriented-Benchmarks)
- [Code Examples](https://github.com/ionq/forte_benchmarking)
- [Code Examples](https://github.com/ionq/forte_aq29_data)
- [SDK](https://docs.ionq.com/sdks/qiskit/index)
- [SDK](https://docs.ionq.com/sdks/cirq/index)
- [SDK](https://docs.ionq.com/sdks/pennylane/index)
- [SDK](https://docs.ionq.com/sdks/qbraid/index)
- [SDK](https://docs.ionq.com/sdks/cuda-q)
- [SDK](https://docs.ionq.com/sdks/tensorflow)
- [Integration](https://aws.amazon.com/braket/quantum-computers/ionq/)
- [Integration](https://azure.microsoft.com/products/quantum/)
- [Integration](https://cloud.google.com/blog/products/compute/ionq-quantum-computing-now-available-on-google-cloud)
- [LinkedIn](https://www.linkedin.com/company/ionq)
- [Twitter](https://x.com/ionq_inc)
- [YouTube](https://www.youtube.com/@ionq_inc)
- [Plans](plans/ionq-plans-pricing.yml)
- [Rate Limits](rate-limits/ionq-rate-limits.yml)
- [Fin Ops](finops/ionq-finops.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
