# HexaGlue

**Focus on business code, not infrastructure glue.**

HexaGlue is a compile-time tool that analyzes the domain of hexagonal applications and generates infrastructure glue around it.

## How it works

1. **Domain analysis**  
   HexaGlue analyzes and models the domain of a hexagonal application at compile time.

2. **Plugin delegation**  
   The analyzed domain model is delegated to specialized plugins through a stable SPI.

3. **Infrastructure generation**  
   Plugins generate the required infrastructure glue code around the domain.

## Key Principles

1. **Your domain stays pure** - HexaGlue never modifies your business code
2. **Zero boilerplate** - Write ports once, infrastructure adapters are generated in seconds, not days
3. **Plugin-based** - Extensible architecture for any technology stack
4. **Compile-time safety** - Generation happens during compilation with full type checking
5. **Replaceable infrastructure** - Swap infrastructure without touching business logic, by switching plugins

## Project structure

The HexaGlue project is organized into three repositories:

1. **[Engine](https://github.com/hexaglue/engine)** - the compile-time analysis and generation core
2. **[Plugins](https://github.com/hexaglue/plugins)** - official infrastructure generators built on a stable SPI
3. **[Examples](https://github.com/hexaglue/examples)** - real-world usage examples and integration scenarios

## Status

- HexaGlue is under active development.
- The core engine and SPI are designed for stability, while new plugins are added incrementally.

---

<div align="center">

**HexaGlue - Focus on business code, not infrastructure glue.**

Made with ❤️ by Scalastic<br>
Copyright 2025 Scalastic - Released under MPL-2.0

</div>