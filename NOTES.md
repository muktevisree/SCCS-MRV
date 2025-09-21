# Methodology, QA & Validation

- **Additivity**: Sum(daily) = Sum(monthly) = Annual injected per facility (validated on this package).
- **Reservoir-type logic**: Basalt/Saline → `co2_produced_tonnes = 0`; Depleted gas → 0.1–5% of injected.
- **Transport loss**: 0 when pipeline length = 0; otherwise constrained to 0.01–0.5% of injected.
- **Leak logic**: leak mass = 0 when 0 events; ≥0.1 t per event otherwise.
- **Capture energy intensity**: per-tech bands (MEA 0.15–0.40; MDEA 0.12–0.35; Selexol/PSA 0.05–0.20; Amine 0.12–0.40 MWh/t).
- **Mass balance**: `co2_net_stored_tonnes = injected − produced − transport_loss − leak_mass` (non-negative enforced).
- **MMV alignment**: Basalt → pressure + (microseismic/4D); Saline → pressure + (tracer/4D); Depleted gas → pressure + (tracer/production logging/well integrity).
- **Geospatial**: WGS84 decimal degrees; synthetic coordinates within US bounds.

This package reflects the final QA corrections applied to the full dataset; monthly is recomputed from daily accordingly.
