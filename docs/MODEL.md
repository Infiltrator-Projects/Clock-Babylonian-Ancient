# Babylonian-Ancient clock — model

**Stable ID:** `babylonian-ancient` · **Kind:** `clock`

## Defined behaviour

Ancient Mesopotamian astronomical time: 12 fixed bēru per nominal 24-hour day, 30 UŠ per bēru (4 SI minutes per UŠ), counted from the most recent computed sunset. Actual sunset intervals vary; the count is not clamped. Requires a valid computed sunset as the daily origin.

**Historical interpretation:** bēru and UŠ elapsed from sunset.

**Fidelity boundary:** Reconstructed coarse measurement, not a named Babylonian civil-era/location chronology.

This resource owns its clock rendering and next visible update boundary. The clock's display mode must not be confused with Common's elapsed-duration projection. Required location inputs must be validated, and unsupported solar events must not be fabricated. Model accuracy must not be overstated beyond this documented interpretation.

## Implementation status

This repository now contains its own clock provider implementation, regression fixtures, Makefile, and independent `.so` build. The Makefile offers release and packaging targets through pinned Common tooling; this does not establish that a GitHub release has already been published. The historical implementation in [Libraries/Common](https://github.com/Infiltrator-Projects/Libraries/tree/main/resources/temporal) remains available for comparison.

## Source documentation

[Calendar's clock model matrix](https://github.com/Infiltrator-Projects/Calendar/blob/main/docs/MODELS.md) · [Historical fidelity audit](https://github.com/Infiltrator-Projects/Libraries/blob/main/docs/TEMPORAL_HISTORICAL_FIDELITY.md) · [Runtime ABI](https://github.com/Infiltrator-Projects/Libraries/blob/main/docs/TEMPORAL_PROVIDERS.md)

## Source provenance

The original Common 1.19.78 extraction is historical evidence. Current builds use the authoritative pinned Common submodule. See [source record](../SOURCE.md) and [recorded results](../VALIDATION-RESULTS.json). The operational model, worked examples and limitations are maintained in [GUIDE.json](GUIDE.json).
