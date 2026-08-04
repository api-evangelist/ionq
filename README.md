# IonQ (ionq)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
