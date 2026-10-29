# Descartes Labs

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Descartes Labs was a Santa Fe, New Mexico geospatial intelligence company founded in 2014 as a spin-out from Los Alamos National Laboratory. The company built the Descartes Labs Platform, a cloud-native geospatial data refinery and analytics environment combining a petabyte-scale satellite imagery archive (Landsat, Sentinel-1/2, MODIS, NAIP, PlanetScope, SkySat, commercial radar, NEXRAD weather radar, plus client-uploaded data) with a Python client library, JupyterHub-based workbench, and distributed compute for training and running deep learning and remote-sensing models at scale. Customers in agriculture, mining, energy, defense, insurance, and the U.S. government used the platform to build production geospatial machine learning pipelines covering crop forecasting, mineral exploration, infrastructure monitoring, methane detection, wildfire response, and ESG reporting. The Platform exposed a Catalog (imagery, bands, products, blobs, events), a Compute service (containerised functions, jobs, schedules), a Vector service (tabular and geospatial features), Dynamic Compute (lazy raster algebra and tiling), Auth, and a `descarteslabs` CLI. In October 2024, EarthDaily Analytics — backed by Antarctica Capital — acquired Descartes Labs and the Descartes Labs Government, Inc. subsidiary, folding the team, customers, and platform into the EarthDaily Constellation programme. The product was rebranded EarthOne in 2025; the `descarteslabs` Python package has been formally discontinued in favour of `earthdaily-earthone` (v5.x), the github.com/descarteslabs organisation has been renamed to `dlarchives`, www.descarteslabs.com is now a parked domain, and the docs.descarteslabs.com developer portal has been retired in favour of EarthDaily-hosted EarthOne documentation. This catalog entry preserves the historical Descartes Labs Platform surface as an archive — see the EarthDaily / EarthOne profile for the active product.

**Areas:** Geospatial · Geospatial Intelligence · Earth Observation · Satellite Imagery · Remote Sensing · Raster · Vectors · GIS · Machine Learning · Geospatial Analytics · Agriculture · Mining

## Descartes Labs on APIs.io

Everything profiled for Descartes Labs is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/descartes-labs/](https://apis.io/providers/descartes-labs/)** — or go straight to one of the APIs or properties below.

### APIs (6)

- [Descartes Labs Platform (Archived)](https://apis.io/apis/descartes-labs/descartes-labs-platform/) — The historical Descartes Labs Platform — a managed geospatial data refinery and analytics environment exposing imagery catalog, raster access, vector…
- [Descartes Labs Catalog API](https://apis.io/apis/descartes-labs/catalog/) — The Catalog organised all imagery and derived data on the Platform. Products group Bands which group Images; Storage Blobs hold arbitrary file artefacts;…
- [Descartes Labs Compute API](https://apis.io/apis/descartes-labs/compute/) — The Compute service ran user-supplied Python code as containerised Functions against the imagery archive at scale. Users defined a `Function` (CPUs, memory,…
- [Descartes Labs Vector API](https://apis.io/apis/descartes-labs/vector/) — The Vector service hosted tabular and geospatial feature data as Tables of typed columns with `uuid` identifiers and ipyleaflet visualisation. Supported…
- [Descartes Labs Dynamic Compute API](https://apis.io/apis/descartes-labs/dynamic-compute/) — Dynamic Compute was the Platform's lazy map-computation engine for interactive raster algebra and tile rendering in notebooks. Expressions over imagery…
- [Descartes Labs Auth API](https://apis.io/apis/descartes-labs/auth/) — The Auth module handled token-based authentication against app.descarteslabs.com — OAuth login flow, refresh tokens, and the user namespace claim that…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Descartes Labs Domain Security](https://apis.io/security/descartes-labs/descartes-labs-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.descarteslabs.com)
- [Documentation](https://docs.descarteslabs.com)
- [Support](https://support.descarteslabs.com)
- [GitHub](https://github.com/dlarchives)

## API Evangelist rating

**Unrated** — none of the rubric's checks were satisfied by anything we could find.

This is not a score of zero. No rating is published for this company. If that is wrong because something public exists that we missed, say so on this repository or email [info@apievangelist.com](mailto:info@apievangelist.com) and it will be re-run — free, and no justification needed.

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Descartes Labs: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/descartes-labs/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
