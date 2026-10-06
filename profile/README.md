# CERTAIN

**Certification for Ethical and Regulatory Transparency in Artificial Intelligence**

CERTAIN develops guidelines and open tools that help data holders, dataspace operators, AI providers and deployers comply with EU regulation: traceable documentation of AI systems, data quality and bias assessment, privacy protection, and preparation for certification under the EU AI Act. The project is funded by the European Union under Horizon Europe (grant agreement 101189650).

## Architecture

![CERTAIN interconnected tool ecosystem: the AIDOC-AP ontology describes the AI/MLOps lifecycle; the Semantic MLOps Engine tracks the lifecycle, stores versioned artefacts and builds a knowledge graph that is an instance of the ontology; a trustworthiness dashboard computes trust scores from the metadata; a data lineage connector exports annotated metadata to the data space, where the RegOps engine queries it to assess compliance with the AI Act and GDPR.](architecture.png)

The **Semantic MLOps Engine** collects (meta)data from every stage of an ML pipeline and stores it as versioned artefacts. Its knowledge graph is an instance of the **AIDOC-AP** ontology, which describes AI systems and their lifecycle along the technical documentation required by Annex IV of the AI Act. The graph is exported to the CERTAIN **data space** through a data lineage connector, and the **RegOps engine** queries it in CI/CD compliance workflows.

## Repositories

**Documentation and traceability of AI systems**

| Repository | What it is |
|---|---|
| [aidoc-ap](https://github.com/CERTAIN-Project/aidoc-ap) | AIDOC-AP, an application profile for the technical documentation of AI systems (Article 11 and Annex IV of the AI Act), with the Annex IV requirements and competency questions. [w3id.org/aidoc-ap](https://w3id.org/aidoc-ap) |
| [aidoc-ap-lifecycle](https://github.com/CERTAIN-Project/aidoc-ap-lifecycle) | AIDOC-AP Lifecycle Extension: terms for all stages of the AI system lifecycle, with worked examples. [Documentation](https://certain-project.github.io/aidoc-ap-lifecycle/) |
| [Semantic_MLOps_engine](https://github.com/CERTAIN-Project/Semantic_MLOps_engine) | Semantic MLOps Engine: MLflow-based capture of lifecycle metadata, exposed as an AIDOC-AP knowledge graph via R2RML and Ontop |
| [aidoc-ap-compliance](https://github.com/CERTAIN-Project/aidoc-ap-compliance) | Compliance dashboard that runs the competency queries against an instantiated knowledge graph and reports what documentation is missing. [Demo](https://certain-project.github.io/aidoc-ap-compliance/) |

**Synthetic data**

| Repository | What it is |
|---|---|
| [Synthetic-Data-Generation-Component](https://github.com/CERTAIN-Project/Synthetic-Data-Generation-Component) | Agent-based simulation that generates realistic public deliberation data |
| [synthetic_energy_data_generation](https://github.com/CERTAIN-Project/synthetic_energy_data_generation) | Preprocessing pipeline and generative model for synthetic residential energy consumption data |
| [empw-synth-data](https://github.com/CERTAIN-Project/empw-synth-data) | Anonymised synthetic smart-meter data for energy communities, with fidelity and privacy evaluation (EMPOWER pilot) |

**Pilots**

| Repository | What it is |
|---|---|
| [empw-enparto](https://github.com/CERTAIN-Project/empw-enparto) | Optimisation and fairness metrics for participation factors in renewable energy communities (EMPOWER pilot) |

## Objectives

- Traceability of critical information about AI systems
- Guidelines for the legally and ethically compliant assessment of AI systems under EU regulation
- Tools for dataspace providers and data holders to comply with AI regulation and reduce energy consumption
- Methods to assess and improve the compliance of AI systems, and certification procedures for them
- Evidence of applicability across sectors through pilots
- An open community around the EU AI ecosystem and related initiatives

---

[Website](https://certain-project.eu/) · [YouTube](https://www.youtube.com/@certain-project) · [Bluesky](https://bsky.app/profile/certainproject.bsky.social) · [LinkedIn](https://www.linkedin.com/company/certain-project) · [Mastodon](https://mastodon.social/@CERTAIN)

<sub>Funded by the European Union. Views and opinions expressed are those of the authors only and do not necessarily reflect those of the European Union. Neither the European Union nor the granting authority can be held responsible for them.</sub>
