# HexaGlue

***Focus on business code, not infrastructure glue.***
<br><br>

> [!NOTE]
> **HexaGlue automatically generates the infrastructure code around your hexagonal architecture, so you can focus on what matters: your business logic.**

## What is HexaGlue?

HexaGlue is a compile-time tool that analyzes your domain code and generates all the infrastructure adapters you need. Write your ports once, and let HexaGlue create the REST controllers, database repositories, message handlers, and more.

```text
┌─────────────────┐                    ┌─────────────────────────────────┐
│  Domain Code    │                    │  Complete Application           │
│                 │     HexaGlue       │                                 │
│  • Ports        │  ──────────────>   │  • Domain Code (unchanged)      │
│  • Use Cases    │    mvn compile     │  • REST Controllers (generated) │
│  • Entities     │                    │  • Repositories (generated)     │
│                 │                    │  • Message Handlers (generated) │
└─────────────────┘                    └─────────────────────────────────┘

 [You write this]                           [HexaGlue generates that]
```

## How it works

HexaGlue works in three simple steps during your build:

1. **Analyze** - Scans your domain code and identifies ports (interfaces your business needs)
2. **Delegate** - Passes the domain model to specialized plugins via a stable SPI
3. **Generate** - Creates infrastructure adapters (REST, database, messaging, etc.) automatically

## Why use HexaGlue?

✅ **Pure domain code** - Your business logic stays clean, with zero infrastructure dependencies

✅ **No boilerplate** - Write a port interface once, get production-ready adapters in seconds

✅ **Type-safe** - Generation happens at compile time with full type checking

✅ **Flexible infrastructure** - Swap technologies (REST to GraphQL, MySQL to MongoDB) by changing plugins, not code

✅ **Extensible** - Add support for any technology through the plugin system

## Getting started

The HexaGlue project is organized into three repositories:

- **[Engine](https://github.com/hexaglue/engine)** - Core analysis and generation engine
- **[Plugins](https://github.com/hexaglue/plugins)** - Official infrastructure generators (REST, JPA, Kafka, etc.)
- **[Examples](https://github.com/hexaglue/examples)** - Real-world usage examples and tutorials

> [!TIP]
> **Start with the [Examples](https://github.com/hexaglue/examples) repository to see HexaGlue in action.**

## Status

HexaGlue is under active development. The core engine and SPI are stable, while new plugins are added regularly.

---

<div align="center">

**HexaGlue - Focus on business code, not infrastructure glue.**

Made with ❤️ by Scalastic<br>
Copyright 2025 Scalastic - Released under MPL-2.0

</div>
