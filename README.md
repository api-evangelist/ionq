# IonQ (ionq)

IonQ (NYSE IONQ) is a College Park, Maryland-based public trapped-ion quantum computing company. IonQ designs, manufactures, and operates trapped-ion quantum computers (Aria, Forte, Forte Enterprise, Tempo, Harmony) and delivers them through the IonQ Quantum Cloud REST API, on-premises Forte Enterprise systems, and partner clouds (AWS Braket, Microsoft Azure Quantum, Google Cloud). The platform supports submission of QIS and native-gate circuits, multi-circuit and Quantum Function jobs, reserved Sessions, error mitigation, and organization-level usage and cost reporting. IonQ's quantum networking, security (QKD), sensing, and space-infrastructure businesses extend the trapped-ion core into a broader quantum systems portfolio.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/ionq/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Quantum Computing, Trapped Ion, QPU, Aria, Forte, Tempo, Quantum Cloud, Cloud, Hardware, Public Company

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Systems

| System | Backend ID | Technology | Notes |
|---|---|---|---|
| IonQ Aria | `qpu.aria-1`, `qpu.aria-2` | Trapped ion | Commercially available QPU |
| IonQ Forte | `qpu.forte-1` | Trapped ion, software-configurable | Limited beta |
| IonQ Forte Enterprise | `qpu.forte-enterprise-1` | Trapped ion | Rack-mounted on-prem |
| IonQ Tempo | n/a (announced) | Trapped ion | Next-generation system |
| IonQ Harmony | (cloud) | Trapped ion | Earlier-generation system |
| IonQ Simulator | `simulator` | Classical | Ideal + noisy, up to 29 qubits |

## APIs

### IonQ Quantum Cloud API
REST API for submitting quantum circuits, managing jobs and sessions, inspecting backends and characterizations, and tracking cost and usage on the IonQ Quantum Cloud.

**Human URL:** [https://docs.ionq.com/api-reference/v0.4/introduction](https://docs.ionq.com/api-reference/v0.4/introduction)
**Base URL:** `https://api.ionq.co/v0.4`
**Authentication:** `Authorization: apiKey $IONQ_API_KEY`

- [Documentation](https://docs.ionq.com/api-reference/v0.4/introduction)
- [Direct API Submission Guide](https://docs.ionq.com/guides/direct-api-submission)
- [OpenAPI](openapi/ionq-quantum-cloud-openapi.yml)
- [JSON Schema — Job](json-schema/ionq-job-schema.json)
- [JSON Schema — Backend](json-schema/ionq-backend-schema.json)
- [JSON Schema — Session](json-schema/ionq-session-schema.json)
- [JSON-LD Context](json-ld/ionq-context.jsonld)
- [JSON Structure — Job](json-structure/ionq-job-structure.json)
- [Naftiko Capability — Jobs](capabilities/quantum-cloud-jobs.yaml)
- [Naftiko Capability — Backends](capabilities/quantum-cloud-backends.yaml)
- [Naftiko Capability — Sessions](capabilities/quantum-cloud-sessions.yaml)
- [Naftiko Capability — Usage](capabilities/quantum-cloud-usage.yaml)
- [Example — Create Job](examples/ionq-create-job-example.json)
- [Example — Get Backends](examples/ionq-get-backends-example.json)
- [Example — Create Session](examples/ionq-create-session-example.json)

### IonQ Quantum Cloud API (v0.3 Legacy)
Previous-generation REST API for jobs, characterizations, backends, and reports. Superseded by v0.4 but still supported.

**Human URL:** [https://docs.ionq.com/api-reference/v0.3/introduction](https://docs.ionq.com/api-reference/v0.3/introduction)
**Base URL:** `https://api.ionq.co/v0.3`

- [Documentation](https://docs.ionq.com/api-reference/v0.3/introduction)
- [Migration v0.3 to v0.4](https://docs.ionq.com/api-reference/v0.4/migration-from-v0.3)

## Resource Coverage (v0.4)

| Resource | Endpoints |
|---|---|
| Jobs | `POST /jobs`, `GET /jobs`, `DELETE /jobs`, `GET /jobs/{id}`, `DELETE /jobs/{id}`, `PUT /jobs/{id}/status/cancel`, `PUT /jobs/status/cancel`, `GET /jobs/{id}/cost`, `GET /jobs/estimate`, `GET /jobs/{id}/circuits/{lang}`, `GET /jobs/{id}/results/probabilities`, `GET /jobs/{id}/variants/{vid}/results/probabilities`, `GET /jobs/{id}/variants/{vid}/results/histogram`, `GET /jobs/{id}/variants/{vid}/results/shots` |
| Backends | `GET /backends`, `GET /backends/{name}`, `GET /backends/{name}/characterizations`, `GET /backends/{name}/characterizations/{id}` |
| Sessions | `POST /sessions`, `GET /sessions`, `GET /sessions/{id}`, `POST /sessions/{id}/end`, `GET /sessions/{id}/jobs` |
| Utility | `GET /whoami`, `GET /organizations/{id}/usage` |

## SDKs and Tools

- [ionq-core](https://github.com/ionq/ionq-core-python) — Apache 2.0 Python client generated from OpenAPI; published to PyPI as `ionq-core`.
- [blqs](https://github.com/ionq/blqs) — Python building blocks for quantum DSLs.
- [pyGSTi](https://github.com/ionq/pyGSTi) — IonQ fork of Gate Set Tomography.
- [qrmi](https://github.com/ionq/qrmi) — Vendor-agnostic Rust layer for quantum resources.
- [torchquantum-dist](https://github.com/ionq/torchquantum-dist) — Multi-GPU statevector QML simulation.
- [QC-App-Oriented-Benchmarks](https://github.com/ionq/QC-App-Oriented-Benchmarks) — QED-C benchmarks.
- [Qiskit](https://docs.ionq.com/sdks/qiskit/index), [Cirq](https://docs.ionq.com/sdks/cirq/index), [PennyLane](https://docs.ionq.com/sdks/pennylane/index), [qBraid](https://docs.ionq.com/sdks/qbraid/index), [CUDA-Q](https://docs.ionq.com/sdks/cuda-q), [TensorFlow Quantum](https://docs.ionq.com/sdks/tensorflow) integrations.

## Partner Clouds

- [AWS Braket](https://aws.amazon.com/braket/quantum-computers/ionq/)
- [Microsoft Azure Quantum](https://azure.microsoft.com/products/quantum/)
- [Google Cloud Marketplace](https://cloud.google.com/blog/products/compute/ionq-quantum-computing-now-available-on-google-cloud)

## Plans, Rate Limits, FinOps

- [Plans and Pricing](plans/ionq-plans-pricing.yml)
- [Rate Limits](rate-limits/ionq-rate-limits.yml)
- [FinOps Surface](finops/ionq-finops.yml)

## Operational Surfaces

- [Quantum Cloud Console](https://cloud.ionq.com)
- [Status](https://status.ionq.co)
- [Support Center](https://support.ionq.com)
- [Newsroom](https://ionq.com/news)
- [Investor Relations (NYSE IONQ)](https://investors.ionq.com)
- [Terms of Service](https://ionq.com/legal/terms-of-service)
- [Privacy Policy](https://ionq.com/legal/privacy-policy)
- [GitHub](https://github.com/ionq)

## Governance Artifacts

- [Spectral Ruleset](rules/ionq-rules.yml)
- [Vocabulary](vocabulary/ionq-vocabulary.yml)
- [Review](review.yml)
