# Lux FHE Handbook

A deep-dive guide to the Lux FHE compiler stack — the IR dialects, the
optimizer, the runtime, and the operational concerns that come with
deploying Fully Homomorphic Encryption.

This is the technical handbook. For the higher-level docs site see
[`luxfhe/docs`](https://github.com/luxfhe/docs); for hands-on tutorials
see [`luxfhe/workshop`](https://github.com/luxfhe/workshop); for code
samples see [`luxfhe/examples`](https://github.com/luxfhe/examples).

## Chapters

### Getting Started

- [Quick Start](./chapters/quick_start.md)
- [Quick Overview](./chapters/quick_overview.md)
- [Installation](./chapters/installing.md)
- [Terminology and Structure](./chapters/terminology.md)

### Compiler Dialects

The compiler is structured as a stack of MLIR dialects, each lowering
into the next.

- [Overview of FHE-related dialects](./chapters/dialects.md)
- [FHE Dialect](./chapters/FHEDialect.md)
- [FHELinalg Dialect](./chapters/FHELinalgDialect.md)
- [TFHE Dialect](./chapters/TFHEDialect.md)
- [Concrete (Torus) Dialect](./chapters/ConcreteDialect.md)
- [Optimizer Dialect](./chapters/OptimizerDialect.md)
- [RT Dialect](./chapters/RTDialect.md)
- [SDFG Dialect](./chapters/SDFGDialect.md)
- [Tracing Dialect](./chapters/TracingDialect.md)
- [TypeInference Dialect](./chapters/TypeInferenceDialect.md)

### Compiler Internals

- [Project layout](./chapters/layout.md)
- [Fusing](./chapters/fusing.md)
- [Crypto-parameter optimizer](./chapters/optimizer.md)
- [Security](./chapters/security.md)
- [Releasing Torus](./chapters/releasing.md)

### Backends

- [Backends overview](./chapters/backends/README.md)
- [Writing a new backend](./chapters/backends/new_backend.md)

### Guides

- [Configure](./chapters/configure.md)
- [Manage Keys](./chapters/manage_keys.md)
- [Deploy](./chapters/deploy.md)
- [Calling from other languages](./chapters/call_from_other_language.md)

### TFHE-rs interop

- [TFHE-rs overview](./chapters/tfhers/README.md)
- [Pregenerated keys](./chapters/tfhers/pregenerated-key.md)
- [Shared keys](./chapters/tfhers/shared-key.md)
- [Serialization](./chapters/tfhers/serialization.md)

### Resources

- [Curated resources](./resources.md) — papers, tutorials, videos

## Related repositories

- [`luxfhe/docs`](https://github.com/luxfhe/docs) — full documentation site
- [`luxfhe/workshop`](https://github.com/luxfhe/workshop) — interactive tutorials
- [`luxfhe/examples`](https://github.com/luxfhe/examples) — code samples across languages
- [`luxfhe/torus`](https://github.com/luxfhe/torus) — the compiler itself

## License

Apache 2.0
