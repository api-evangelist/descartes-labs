# Descartes Labs (descartes-labs)

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

Descartes Labs was a Santa Fe, New Mexico geospatial intelligence company (founded 2014, spin-out from Los Alamos National Laboratory) that built a cloud-native geospatial data refinery — a petabyte-scale satellite imagery archive plus Python client, JupyterHub workbench, Catalog, Compute, Vector, and Dynamic Compute services — used by enterprise and U.S. government customers for production geospatial machine learning across agriculture, mining, energy, defense, insurance, and ESG monitoring. EarthDaily Analytics (backed by Antarctica Capital) acquired Descartes Labs in October 2024; the product has since been rebranded **EarthOne**, the `descarteslabs` Python package has been discontinued in favour of `earthdaily-earthone`, the GitHub org `descarteslabs` has been renamed to `dlarchives`, and `www.descarteslabs.com` is now a parked domain. This catalog entry preserves the historical Descartes Labs Platform surface.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/descartes-labs/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Geospatial, Geospatial Intelligence, Earth Observation, Satellite Imagery, Remote Sensing, Raster, Vector, GIS, Machine Learning, Geospatial Analytics, Agriculture, Mining, Energy, Defense, Climate, Acquired, EarthOne, EarthDaily, Discontinued

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## Status

| Field | Value |
|---|---|
| Company status | Acquired by EarthDaily Analytics — October 2024 |
| Product status | Discontinued, rebranded as EarthDaily **EarthOne** |
| Python package | `descarteslabs` 4.0.0.post2 (Dec 2025) — final release, marked **Discontinued. Please use `earthdaily-earthone` instead** |
| Successor package | [`earthdaily-earthone`](https://github.com/earthdaily/earthone-python) 5.x |
| GitHub org | github.com/descarteslabs renamed to [github.com/dlarchives](https://github.com/dlarchives) |
| Website | www.descarteslabs.com — parked / domain landing page |
| Docs | docs.descarteslabs.com — retired (DNS removed) |
| Subsidiary | Descartes Labs Government, Inc. — folded into EarthDaily |

## APIs

The historical platform was a managed geospatial data refinery exposed through the `descarteslabs` Python client. No public OpenAPI specification was ever published — REST endpoints under `*.descarteslabs.com` were considered an implementation detail of the SDK.

### Descartes Labs Platform (Archived)
The historical Descartes Labs Platform — cloud-native geospatial data refinery exposing imagery catalog, raster access, vector tables, compute functions, and authentication via a Python client library, `descarteslabs` CLI, and REST endpoints under `*.descarteslabs.com`. Discontinued in 2025.

- [Source — descarteslabs-python](https://github.com/dlarchives/descarteslabs-python)
- [PyPI — descarteslabs](https://pypi.org/project/descarteslabs/)
- [Successor — earthdaily-earthone](https://github.com/earthdaily/earthone-python)

### Descartes Labs Catalog API
Products, Bands, Images, Storage Blobs, and Events. Sharing model with owners / writers / readers and EventSubscriptions (SQS, ComputeFunctionCompleted, NewImage, NewStorage, NewVector) plus calendar-based EventSchedules.

- [Source — descarteslabs/catalog](https://github.com/dlarchives/descarteslabs-python/tree/master/descarteslabs/catalog)

### Descartes Labs Compute API
Containerised Python `Function` definitions (CPUs, memory, environment) executed as `Job`s — often via `Function.map` over hundreds of thousands of tiles — with `compute-function-completed` events on drain-to-zero.

- [Source — descarteslabs/compute](https://github.com/dlarchives/descarteslabs-python/tree/master/descarteslabs/compute)

### Descartes Labs Vector API
Tabular and geospatial feature `Table`s with typed columns, `uuid` identifiers, property filtering (including `ilike`), and ipyleaflet tile visualisation. Folded into the main client in 3.0.0.

- [Source — descarteslabs/vector](https://github.com/dlarchives/descarteslabs-python/tree/master/descarteslabs/vector)
- [Source — descarteslabs-vector (legacy)](https://github.com/dlarchives/descarteslabs-vector)

### Descartes Labs Dynamic Compute API
Lazy map-computation engine for interactive raster algebra and on-demand XYZ tile rendering in notebooks. Distributed as the standalone `descarteslabs-dynamic-compute` package.

- [Source — descarteslabs-dynamic-compute](https://github.com/dlarchives/descarteslabs-dynamic-compute)
- [PyPI — descarteslabs-dynamic-compute](https://pypi.org/project/descarteslabs-dynamic-compute/)

### Descartes Labs Auth API
OAuth token flow against `app.descarteslabs.com`, refresh handling, and the user-namespace global identifier consumed by every other client module.

- [Source — descarteslabs/auth](https://github.com/dlarchives/descarteslabs-python/tree/master/descarteslabs/auth)

## Migration

EarthDaily provides a migration path from `descarteslabs` to `earthdaily-earthone`:

- `import descarteslabs as dl` → `import earthdaily.earthone as dl`
- `*.descarteslabs.com` URLs → `*.earthone.earthdaily.com` / `*.earthdaily.com`
- Catalog / Vector product prefix `descarteslabs:` → `earthdaily:`
- `DESCARTESLABS_*` environment variables → `EARTHONE_*`

See [github.com/earthdaily/earthone-python](https://github.com/earthdaily/earthone-python) for the active client.

## Common

- [Website (parked)](https://www.descarteslabs.com)
- [Documentation (retired)](https://docs.descarteslabs.com)
- [Support (retired)](https://support.descarteslabs.com)
- [Sign-in app](https://app.descarteslabs.com)
- [GitHub organisation — dlarchives](https://github.com/dlarchives)
- [Python client — descarteslabs-python](https://github.com/dlarchives/descarteslabs-python)
- [PyPI — descarteslabs](https://pypi.org/project/descarteslabs/)
- [Tutorials](https://github.com/dlarchives/tutorials)
- [Example notebooks](https://github.com/dlarchives/example-notebooks)
- [Workflows examples](https://github.com/dlarchives/workflows-examples)
- [Enterprise Accelerator onboarding notebooks](https://github.com/dlarchives/descarteslabs-ea-notebooks)
- [DL-COVID-19 mobility dataset](https://github.com/dlarchives/DL-COVID-19)
- [Contrastive Sensor Fusion research](https://github.com/dlarchives/contrastive_sensor_fusion)
- [Successor — EarthDaily EarthOne Python client](https://github.com/earthdaily/earthone-python)
- [Successor — EarthDaily Analytics](https://earthdaily.com)
- [Acquisition announcement — EarthDaily (Oct 2024)](https://earthdaily.com/blog/descartes-labs-acquisition)
- [Acquisition — PR Newswire](https://www.prnewswire.com/news-releases/earthdaily-analytics-announces-acquisition-of-descartes-labs-302276388.html)

## Maintainers

- **Kin Lane** — kin@apievangelist.com
