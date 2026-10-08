# Urvarā Living Field Twin: open kit

An open toolkit for building auditable, living digital twins of farm landscapes on **OGC 3D Tiles 1.1** and **CesiumJS**.

Most digital twins model the built world as snapshots. This kit models the working landscape: every parcel, its season-by-season history, and the evidence behind every AI-generated flag, streamed in 3D and honest by design.

Built by [BIMSaarthi Technologies Pvt. Ltd.](https://bimsaarthi.com), a DPIIT-recognised deep-tech startup incubated at Ratan Tata Innovation Hub, Mangalagiri, Amaravati, India.

> **Status:** early. The schema stub is here; components land on the schedule in [ROADMAP.md](ROADMAP.md).

## What the kit will contain

| Component | What it does |
|---|---|
| **Agri metadata schema** | 3D Tiles 1.1 metadata for parcels, seasons, indicators, uncertainty, honesty flags and scenario branches |
| **Lineage-in-tile convention** | Carries W3C PROV-O lineage in feature metadata, so every value points to the scenes, dates and rule or model that produced it |
| **Converter** | GeoParquet or GeoSPARQL parcels, terrain and seasonal indices to 3D Tiles 1.1 (`EXT_mesh_features`, `EXT_structural_metadata`, implicit tiling), updated per season |
| **CesiumJS viewer module** | Styling by crop health, drought and sowing status; season slider and history playback; English and Telugu |
| **Provenance panel** | "Why is this parcel flagged?", from evidence to decision, on click |
| **Agent interface** | A model output adapter and an MCP server so any model or AI agent can read the twin and write validated, lineage-bearing predictions |
| **Open pilot twin** | A public pilot for a Mangalagiri cluster (Andhra Pradesh) built from open data only |

## Design principles

- **A memory, not a map.** Append-only history per parcel and season. Corrections are new entries that point at what they correct.
- **Honest rendering.** Uncertainty, native sensor resolution, "no valid observation" under cloud, and relative rank versus absolute value each have a distinct visual treatment.
- **Scale honesty.** Each layer is drawn only at the scale its sensor can defend.
- **Bring your own intelligence.** The kit carries and shows results; it does not require any particular model. Plug in your own models, rules or crop maps.

## Open vs proprietary

**Open (this repository):** schema, lineage convention, converter, viewer module, provenance panel, model adapter, MCP server, pilot data and tutorials.

**Not in this repository:** BIMSaarthi's trained models and weights, inference engines, behavioural intelligence and simulation engines, full ontology and rule base, and agent orchestration. The kit runs without any of them.

No farmer data or government data is published here.

## Data sources for the open pilot

Sentinel-1 and Sentinel-2 (via Copernicus Data Space), CHIRPS rainfall, Copernicus DEM, ESA WorldCover, and open field boundaries. Official cadastral data is used only with state permission.

## Licence

- Code: [Apache License 2.0](LICENSE)
- Schema, documentation and pilot data: CC BY 4.0

## Contact

BIMSaarthi Technologies Pvt. Ltd. · community@bimsaarthi.com · https://bimsaarthi.com

Questions, ideas and contributions are welcome on GitHub Issues or in the BIMSaarthi community: https://community.bimsaarthi.com
