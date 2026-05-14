# Choice of Law Dataverse (CoLD)

Open-access knowledge base on choice of law in international contracts, developed at the [University of Lucerne](https://www.unilu.ch/en/). Winner of the [Swiss National ORD Prize 2025](https://ord.swiss-academies.ch/news/swiss-national-ord-prize-2025-for-legal-and-environmental-sciences).

**[cold.global](https://cold.global)** | **[API docs](https://api.cold.global/api/v1/docs)** | **[Tech Wiki](https://choice-of-law-dataverse.github.io/)**

---

## What is CoLD?

CoLD is a curated repository of private international law data covering **63+ jurisdictions** worldwide. It helps researchers, practitioners, and students explore choice-of-law rules across legal systems through structured, comparable data.

- **Repository** — carefully curated private international law data, kept up to date as legal systems evolve.
- **Community** — a network of specialists, researchers, and practitioners who transform data points into knowledge.
- **Open Research** — all data licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), promoting sharing, citing, exploring, and analyzing research data on choice of law.

## Available datasets

| Dataset | Description |
|---|---|
| **Answers** | Country-level responses to the CoLD standardised questionnaire on choice-of-law rules |
| **HCCH Answers** | Answers mapped to the HCCH Principles on Choice of Law |
| **Questions** | The standardised questionnaire items that Answers respond to |
| **Court Decisions** | Case law with metadata, themes, PIL provisions, and jurisdiction links |
| **Domestic Instruments** | National statutes, codes, and PIL regulations |
| **Domestic Legal Provisions** | Individual articles/provisions within domestic instruments |
| **Regional Instruments** | Supranational instruments (e.g. EU Rome I Regulation) |
| **Regional Legal Provisions** | Individual articles/provisions within regional instruments |
| **International Instruments** | Treaties, conventions, and model laws (e.g. HCCH Principles) |
| **International Legal Provisions** | Individual articles/provisions within international instruments |
| **Literature** | Academic and practitioner publications on choice of law |
| **Arbitral Awards** | Published arbitral awards with choice-of-law analysis |
| **Arbitral Rules** | Institutional arbitration rules (e.g. ICC, LCIA) |
| **Arbitral Provisions** | Individual articles within arbitral rules |
| **Arbitral Institutions** | Arbitration institutions (e.g. ICC, SIAC) |
| **Jurisdictions** | Countries and territories with metadata (region, legal family) |
| **Specialists** | Choice-of-law experts by jurisdiction |

Bulk CSV and XLSX exports are available at [cold.global/data-sets](https://cold.global/data-sets).

## Open API

Read-only data endpoints are **publicly accessible** — no API key or token required.

```bash
# Search across all datasets
curl "https://api.cold.global/api/v1/search/?search_string=party+autonomy"

# Export an entire table
curl "https://api.cold.global/api/v1/search/full_table?table=Court+Decisions"

# Fetch a single record with related entities
curl "https://api.cold.global/api/v1/search/details?table=Court+Decisions&id=CD-CHE-42"
```

Full interactive documentation: [api.cold.global/docs](https://api.cold.global/docs)

## Repositories

| Repository | Description |
|---|---|
| [**cold-web-app**](https://github.com/Choice-of-Law-Dataverse/cold-web-app) | Nuxt 4 frontend + FastAPI backend powering [cold.global](https://cold.global) |
| [**Choice-of-Law-Dataverse.github.io**](https://github.com/Choice-of-Law-Dataverse/Choice-of-Law-Dataverse.github.io) | Technical documentation and architecture wiki |

## Contributing

We welcome contributions that improve the quality and usability of our projects.

1. Fork the repository and clone your fork locally.
2. Create a feature branch: `feature/short-description`.
3. Commit using [Conventional Commits](https://www.conventionalcommits.org/): `type(scope): description`.
4. Open a pull request against `main` for review.

For data contributions (country reports, specialist reviews), see [cold.global/contact](https://cold.global/contact).

## Learn more

- [Glossary](https://cold.global/learn/glossary) — key private international law terms (party autonomy, depeçage, mandatory rules, etc.)
- [Methodology](https://cold.global/learn/methodology) — how the CoLD questionnaire is structured and data is collected
- [FAQ](https://cold.global/learn/faq) — common questions about choice of law and the Dataverse
- [Open Educational Resources](https://cold.global/learn/open-educational-resources) — curated readings and publications

## Contact

**Choice of Law Dataverse — University of Lucerne**
Inseliquai 8, Room INS-1, 6005 Luzern, Switzerland
[mail@cold.global](mailto:mail@cold.global) | [LinkedIn](https://www.linkedin.com/company/choice-of-law-dataverse/) | [Newsletter](https://choiceoflawdataverse.substack.com/)

---

Licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). An [SNF-funded](https://www.snf.ch/) project at the University of Lucerne.
