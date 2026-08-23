# Modified Booth Algorithm

This section documents the algorithm used by the 4×4 Modified Booth multiplier.

## Radix-4 Recoding

Modified Booth encoding processes two multiplier bits at a time while examining an overlapping three-bit group. The encoding produces one of five signed operations:

- `0`
- `+M`
- `−M`
- `+2M`
- `−2M`

## Encoding Table

| Three-bit group | Operation |
|---|---|
| 000 | 0 |
| 001 | +M |
| 010 | +M |
| 011 | +2M |
| 100 | −2M |
| 101 | −M |
| 110 | −M |
| 111 | 0 |

## Implementation Mapping

The repository will connect the algorithmic operations to the actual transistor-level schematic blocks after the Cadence screenshots are added.
