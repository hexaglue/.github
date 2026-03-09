# HexaGlue

***Compile your architecture, not just your code.***

**[hexaglue.io](https://hexaglue.io)** · Core `6.1.0` · Plugins `3.1.0` · License `MPL-2.0`

---

HexaGlue is an **architecture compiler** for Java applications. At compile time, it parses your source code, classifies domain concepts (aggregates, ports, value objects…), and feeds an architectural model to plugins that **audit**, **document**, and **generate infrastructure**.

One `mvn compile`. Architecture analyzed, validated, and generated.

## Repositories

| Repository | Description |
|------------|-------------|
| **[hexaglue](https://github.com/hexaglue/hexaglue)** | Core engine, plugins, Maven plugin, and examples |
| **[case-study-ecommerce](https://github.com/hexaglue/case-study-ecommerce)** | E-commerce migration: mono-module, Java 17 |
| **[case-study-banking](https://github.com/hexaglue/case-study-banking)** | Banking migration: multi-module, Java 21 |
| **[case-study-lombok](https://github.com/hexaglue/case-study-lombok)** | Lombok support validation |

## Get Started

**[Documentation](https://hexaglue.io/docs/getting-started/)** · **[Case Studies](https://hexaglue.io/case-studies/)**

```xml
<plugin>
  <groupId>io.hexaglue</groupId>
  <artifactId>hexaglue-maven-plugin</artifactId>
  <version>6.1.0</version>
</plugin>
```

---

<div align="center">

**[hexaglue.io](https://hexaglue.io)**

Made with ❤️ by Scalastic<br>
Copyright 2026 Scalastic - Released under MPL-2.0

</div>
