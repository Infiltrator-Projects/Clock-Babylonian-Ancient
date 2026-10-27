# Babylonian-Ancient clock — model

**Stable ID:** `babylonian-ancient` · **Kind:** `clock`

## Defined behaviour

Ancient Mesopotamian astronomical time: 12 fixed bēru per sunset-to-sunset day, 30 UŠ per bēru (4 SI minutes per UŠ). Requires a valid computed sunset as the daily origin.

**Historical interpretation:** bēru and UŠ elapsed from sunset.

**Fidelity boundary:** Reconstructed coarse measurement, not a named Babylonian civil-era/location chronology.

This resource owns its clock rendering and next visible update boundary. The clock's display mode must not be confused with Common's elapsed-duration projection. Required location inputs must be validated, and unsupported solar events must not be fabricated. Model accuracy must not be overstated beyond this documented interpretation.

## Implementation status

The source, tests and combined package still belong to [Libraries/Common](https://github.com/Infiltrator-Projects/Libraries/tree/main/resources/temporal). This repository documents the independent `.so` resource that is intended to be migrated; it does **not** claim a working standalone installer or release.

## Source documentation

[Calendar's clock model matrix](https://github.com/Infiltrator-Projects/Calendar/blob/main/docs/MODELS.md) · [Historical fidelity audit](https://github.com/Infiltrator-Projects/Libraries/blob/main/docs/TEMPORAL_HISTORICAL_FIDELITY.md) · [Runtime ABI](https://github.com/Infiltrator-Projects/Libraries/blob/main/docs/TEMPORAL_PROVIDERS.md)

## Source copy status

The model-specific implementation and required helpers are now copied into this repository. Its behaviour was compared with the original Common 1.19.78 provider; this adds copy-regression evidence, not a new independent historical audit. See [source provenance](../SOURCE.md) and [validation results](../VALIDATION-RESULTS.json). The original Common implementation remains in place.
