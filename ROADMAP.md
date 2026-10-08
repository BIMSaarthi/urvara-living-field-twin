# Roadmap

Months are counted from project start. Dates are targets.

| Month | Milestone | Deliverable |
|---|---|---|
| 1 | Repository and open data | Repository live; open data pulled for the Mangalagiri pilot cluster |
| 2 | **M1: Schema and lineage convention** | Agri 3D Tiles 1.1 metadata schema (including scenario branch convention) and lineage-in-tile convention published; review requested from the 3D Tiles community |
| 3 | Converter alpha | Implicit tiling, per-season property tables, terrain draping; first tests against the vector tiles technology preview |
| 4 | **M2: Converter v0.1** | Converter release with GeoParquet input and per-season updates; pilot tileset published; benchmark of at least 1 million open or synthetic parcels |
| 5 | Viewer | Styling by crop health, drought and sowing status; season slider; field validation begins |
| 6 | **M3: Viewer, provenance, agents** | CesiumJS viewer module, provenance panel, model adapter and MCP server v0.1 |
| 7 | Honesty styling | Honesty styling library; season-history playback |
| 8 | **M4: Season history and field check** | Season-history playback released; de-identified field validation summary; Telugu interface; tutorial 1 |
| 9 | **Final: Public living twin** | Public pilot twin live on open data; tutorial 2; final report |

## Stretch goals

- One worked what-if scenario with split-view comparison
- Water-column voxel layer (`EXT_primitive_voxels`) from public reanalysis and well data
- Field photos anchored as camera poses or Gaussian splats

## Beyond the first release

Federated twins where each state or country hosts its own tiles under its own control, and submission of the agri profile as an OGC community practice once at least two independent organisations use it.
