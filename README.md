# Koiwai Schema
Constrained but Adaptable SQL Schema for 4chan Archival Tools

## Design Principles

- Constraints should specify how fields are to be stored.
- Constraints should not impede storage or migrations of possibly flawed or incomplete data, that would just screw us over.
- Clarity first, performance and convenience second.
- Trade-offs between performance and convenience should be evaluated case by case, i.e. storing hashes as TEXT (extremely convenient, extremely bad performance) versus storing hashes as BYTEA (somewhat convenient, moderate performance) versus storing hashes as UUIDs (extremely inconvenient, peak performance).

