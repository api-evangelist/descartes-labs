# Descartes Labs (descartes-labs)
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
