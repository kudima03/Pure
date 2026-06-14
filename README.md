# Pure

Home repository for the **Pure ecosystem** — a collection of immutable, composable, AOT-compatible .NET libraries.

Clone with all submodules:

```sh
git clone --recurse-submodules https://github.com/kudima03/Pure.git
```

Or, after a plain clone:

```sh
git submodule update --init --recursive
```

---

## Repositories

### Primitives

| Repository | Description |
|---|---|
| [Pure.Primitives.Abstractions](https://github.com/kudima03/Pure.Primitives.Abstractions) | Base interfaces for the Pure ecosystem — immutable, composable abstractions over .NET primitive types; AOT-compatible. |
| [Pure.Primitives](https://github.com/kudima03/Pure.Primitives) | Concrete implementations of immutable, composable primitive types for the Pure ecosystem — type-safe wrappers over .NET primitive types; AOT-compatible. |
| [Pure.Primitives.Materialized](https://github.com/kudima03/Pure.Primitives.Materialized) | Eagerly evaluated Pure primitive wrappers — MaterializedBool, MaterializedString, MaterializedNumber, MaterializedGuid, MaterializedDate, MaterializedTime, and more. |
| [Pure.Primitives.Cached](https://github.com/kudima03/Pure.Primitives.Cached) | Memoized Pure primitive wrappers — CachedBool, CachedString, CachedNumber, CachedGuid, CachedDate, CachedTime, CachedDateTime, and others. |
| [Pure.Primitives.Choices](https://github.com/kudima03/Pure.Primitives.Choices) | Conditional selection types for Pure primitives — BoolChoice, StringChoice, NumberChoice, GuidChoice, DateChoice, TimeChoice, DateTimeChoice, and CharChoice. |
| [Pure.Primitives.Switches](https://github.com/kudima03/Pure.Primitives.Switches) | Switch-based conditional primitives for the Pure ecosystem — evaluate one of N branches based on a discriminant value. |
| [Pure.Primitives.Random](https://github.com/kudima03/Pure.Primitives.Random) | Random value generators for Pure primitive types — RandomChar, RandomDate, RandomTime, RandomDateTime, RandomNumber, and collection variants. |

### Primitive Operations

| Repository | Description |
|---|---|
| [Pure.Primitives.Bool.Operations](https://github.com/kudima03/Pure.Primitives.Bool.Operations) | Boolean operations for Pure IBool primitives — And, Or, Xor, Not, BitwiseAnd, BitwiseOr, and equality conditions. |
| [Pure.Primitives.Char.Operations](https://github.com/kudima03/Pure.Primitives.Char.Operations) | Character classification and comparison operations for Pure IChar primitives — IsDigit, IsLetter, IsUpper, IsLower, EqualCondition, and more. |
| [Pure.Primitives.String.Operations](https://github.com/kudima03/Pure.Primitives.String.Operations) | String operations for Pure IString primitives — concatenation, joining, comparison conditions, substring, and hex encoding. |
| [Pure.Primitives.Number.Operations](https://github.com/kudima03/Pure.Primitives.Number.Operations) | Composable arithmetic and comparison value objects over any INumber\<T\> for the Pure ecosystem — lazy, immutable sealed records. |
| [Pure.Primitives.Date.Operations](https://github.com/kudima03/Pure.Primitives.Date.Operations) | Immutable, composable date operations for the Pure ecosystem — comparison conditions and utilities over IDate primitives. |
| [Pure.Primitives.Time.Operations](https://github.com/kudima03/Pure.Primitives.Time.Operations) | Temporal comparison conditions for Pure ITime primitives — Before, After, NotBefore, NotAfter, Equal, NotEqual, and a TimeComparer. |
| [Pure.Primitives.DateTime.Operations](https://github.com/kudima03/Pure.Primitives.DateTime.Operations) | Temporal comparison conditions and ordering checks for IDateTime values in the Pure ecosystem — six IBool condition types. |

### Primitives — Serialization & EF Core

| Repository | Description |
|---|---|
| [Pure.Primitives.Abstractions.Serialization.System](https://github.com/kudima03/Pure.Primitives.Abstractions.Serialization.System) | System.Text.Json converters for Pure.Primitives abstract types — serialize and deserialize IBool, IChar, IString, INumber\<T\>, IGuid, IDate, ITime, IDateTime. |
| [Pure.Primitives.Abstractions.EFCore.Converters](https://github.com/kudima03/Pure.Primitives.Abstractions.EFCore.Converters) | EF Core ValueConverter implementations for Pure.Primitives — maps Pure primitive interfaces to .NET types for database storage. |
| [Pure.Primitives.Abstractions.EFCore.ValueComparers](https://github.com/kudima03/Pure.Primitives.Abstractions.EFCore.ValueComparers) | EF Core ValueComparer implementations for Pure.Primitives — correct change-tracking for Pure primitive types stored via EF Core. |
| [Pure.Primitives.Abstractions.OpenAPI.Schema](https://github.com/kudima03/Pure.Primitives.Abstractions.OpenAPI.Schema) | OpenAPI document transformer for the Pure ecosystem — replaces abstract primitive interface schemas with native OpenAPI type representations. |

### Hash Codes

| Repository | Description |
|---|---|
| [Pure.HashCodes.Abstractions](https://github.com/kudima03/Pure.HashCodes.Abstractions) | Base IDeterminedHash interface for the Pure hash code ecosystem — a byte-enumerable contract for deterministic hash sequences. |
| [Pure.HashCodes](https://github.com/kudima03/Pure.HashCodes) | Deterministic hash code generation for the Pure ecosystem — stable, byte-enumerable hashes over immutable primitive types via DeterminedHash. |

### Collections & LINQ

| Repository | Description |
|---|---|
| [Pure.Collections.Generic](https://github.com/kudima03/Pure.Collections.Generic) | Generic collection types for the Pure ecosystem — Dictionary, Set, Array, OrderedDictionary, and Lookup backed by IDeterminedHash equality. |
| [Pure.Linq.Conditions](https://github.com/kudima03/Pure.Linq.Conditions) | LINQ-compatible IBool conditions over IEnumerable\<T\> sequences for the Pure ecosystem — Empty, NotEmpty, Equal, and NotEqual. |

### Serialization

| Repository | Description |
|---|---|
| [Pure.Serialization.Json](https://github.com/kudima03/Pure.Serialization.Json) | JSON serialization utilities for the Pure ecosystem. |

### Relational Schema

| Repository | Description |
|---|---|
| [Pure.RelationalSchema.Abstractions](https://github.com/kudima03/Pure.RelationalSchema.Abstractions) | Immutable, composable interfaces for relational database schema metadata — schemas, tables, columns, column types, indexes, and foreign keys. |
| [Pure.RelationalSchema](https://github.com/kudima03/Pure.RelationalSchema) | Concrete implementations of the relational schema domain model — schemas, tables, columns, indexes, and foreign keys using Pure.Primitives. |
| [Pure.RelationalSchema.HashCodes](https://github.com/kudima03/Pure.RelationalSchema.HashCodes) | Deterministic hash implementations for relational schema components — schemas, tables, columns, indexes, and foreign keys as composable IDeterminedHash byte sequences. |
| [Pure.RelationalSchema.Conditions](https://github.com/kudima03/Pure.RelationalSchema.Conditions) | IBool condition types over relational schema components for the Pure ecosystem. |
| [Pure.RelationalSchema.Random](https://github.com/kudima03/Pure.RelationalSchema.Random) | Random value generators for relational schema components in the Pure ecosystem — schemas, tables, columns, indexes, and foreign keys. |
| [Pure.RelationalSchema.Abstractions.Serialization.System](https://github.com/kudima03/Pure.RelationalSchema.Abstractions.Serialization.System) | System.Text.Json converters for Pure.RelationalSchema abstract types — ISchema, ITable, IColumn, IColumnType, IForeignKey, and IIndex. |
| [Pure.RelationalSchema.Abstractions.OpenAPI.Schema](https://github.com/kudima03/Pure.RelationalSchema.Abstractions.OpenAPI.Schema) | OpenAPI document transformer for Pure.RelationalSchema.Abstractions — corrects schema components for IColumn, IIndex, ITable, IForeignKey, and ISchema. |

### Relational Schema — Relational & Rich Relational Model

| Repository | Description |
|---|---|
| [Pure.RelationalSchema.RelationalModel.Abstractions](https://github.com/kudima03/Pure.RelationalSchema.RelationalModel.Abstractions) | Relational model interfaces for database schema structures — schemas, tables, columns, indexes, and foreign keys with GUID identity. |
| [Pure.RelationalSchema.RichRelationalModel.Abstractions](https://github.com/kudima03/Pure.RelationalSchema.RichRelationalModel.Abstractions) | Unified schema + relational-model interfaces for the Pure ecosystem — merges structural schema with relational model identity into single composable contracts. |
| [Pure.RelationalSchema.RichRelationalModel.EFCore.Models](https://github.com/kudima03/Pure.RelationalSchema.RichRelationalModel.EFCore.Models) | EF Core models implementing the Rich Relational Model abstractions for database schema introspection in the Pure ecosystem. |
| [Pure.RelationalSchema.RichRelationalModel.EFCore.Models.Configurations](https://github.com/kudima03/Pure.RelationalSchema.RichRelationalModel.EFCore.Models.Configurations) | EF Core IEntityTypeConfiguration\<T\> implementations for the Pure rich relational schema model — schemas, tables, columns, column types, indexes, and foreign keys. |

### Relational Schema — Storage

| Repository | Description |
|---|---|
| [Pure.RelationalSchema.Storage.Abstractions](https://github.com/kudima03/Pure.RelationalSchema.Storage.Abstractions) | Base interfaces for reading stored relational schema data — ICell, IRow, IStoredTableDataSet, and IStoredSchemaDataSet; AOT-compatible. |
| [Pure.RelationalSchema.Storage](https://github.com/kudima03/Pure.RelationalSchema.Storage) | Concrete implementations of stored relational schema data types for the Pure ecosystem — Cell, Row, and StoredSchemaDataset. |
| [Pure.RelationalSchema.Storage.HashCodes](https://github.com/kudima03/Pure.RelationalSchema.Storage.HashCodes) | Deterministic hash code implementations for relational schema storage types — Cell, Row, IStoredTableDataSet, and IStoredSchemaDataSet. |
| [Pure.RelationalSchema.Storage.Abstractions.Serialization.System](https://github.com/kudima03/Pure.RelationalSchema.Storage.Abstractions.Serialization.System) | System.Text.Json converters for relational schema storage abstractions — ICell, IRow, IStoredTableDataSet, and IStoredSchemaDataSet. |
| [Pure.RelationalSchema.Storage.Abstractions.OpenAPI.Schema](https://github.com/kudima03/Pure.RelationalSchema.Storage.Abstractions.OpenAPI.Schema) | OpenAPI document transformer for Pure — corrects auto-generated schemas for ICell, IRow, IStoredTableDataSet, and IStoredSchemaDataSet. |
| [Pure.RelationalSchema.Storage.PostgreSQL](https://github.com/kudima03/Pure.RelationalSchema.Storage.PostgreSQL) | PostgreSQL storage implementation for the Pure relational schema ecosystem — DDL execution, row access, and row insertion via IDbConnection. |
| [Pure.RelationalSchema.Storage.PureQL.Projection](https://github.com/kudima03/Pure.RelationalSchema.Storage.PureQL.Projection) | Executes PureQL queries against in-memory relational schema datasets — translates a Query AST into a LINQ-backed IStoredTableDataSet. |

### Relational Schema — Self-Description

| Repository | Description |
|---|---|
| [Pure.RelationalSchema.Self.Schema](https://github.com/kudima03/Pure.RelationalSchema.Self.Schema) | Concrete ISchema that self-describes the relational schema metadata model — the database schema for a schema registry with 13 tables and 17 foreign keys. |
| [Pure.RelationalSchema.Self.Storage.Projection](https://github.com/kudima03/Pure.RelationalSchema.Self.Storage.Projection) | Projects an ISchema into normalized storage rows for the Pure relational schema meta-model. |
| [Pure.RelationalSchema.Self.Storage.Introjection](https://github.com/kudima03/Pure.RelationalSchema.Self.Storage.Introjection) | Converts relational schema storage rows into a LINQ-queryable IQueryable\<ISchema\> object graph — schema introspection over IStoredSchemaDataSet. |

### Chart Model

| Repository | Description |
|---|---|
| [Pure.Chart.Model.Abstractions](https://github.com/kudima03/Pure.Chart.Model.Abstractions) | Chart model interfaces for the Pure ecosystem — immutable, composable abstractions over chart data structures; AOT-compatible. |
| [Pure.Chart.Model](https://github.com/kudima03/Pure.Chart.Model) | Concrete immutable record implementations of the chart domain model for the Pure ecosystem — implements Pure.Chart.Model.Abstractions contracts. |
| [Pure.Chart.Model.HashCodes](https://github.com/kudima03/Pure.Chart.Model.HashCodes) | Deterministic hash code implementations for chart model abstractions in the Pure ecosystem. |
| [Pure.Chart.RelationalModel.Abstractions](https://github.com/kudima03/Pure.Chart.RelationalModel.Abstractions) | Relational-model interfaces for chart entities in the Pure ecosystem — immutable contracts for charts, types, series, and axes. |
| [Pure.Chart.RelationalModel](https://github.com/kudima03/Pure.Chart.RelationalModel) | Concrete relational model records for the Pure ecosystem — immutable implementations of chart, axis, and series domain entities. |
| [Pure.Chart.RelationalModel.HashCodes](https://github.com/kudima03/Pure.Chart.RelationalModel.HashCodes) | Deterministic hash code implementations for chart relational model entities in the Pure ecosystem. |
| [Pure.Chart.RelationalModel.Abstractions.Serialization.System](https://github.com/kudima03/Pure.Chart.RelationalModel.Abstractions.Serialization.System) | System.Text.Json converters for chart relational model abstractions in the Pure ecosystem. |
| [Pure.Chart.RichRelationalModel.Abstractions](https://github.com/kudima03/Pure.Chart.RichRelationalModel.Abstractions) | Combined chart domain-model and relational-model interfaces for the Pure ecosystem — rich view with both navigation properties and FK identity. |
| [Pure.Chart.RichRelationalModel](https://github.com/kudima03/Pure.Chart.RichRelationalModel) | Concrete immutable record implementations of the rich relational chart model for the Pure ecosystem — carries both FK IDs and resolved navigations. |
| [Pure.Chart.RichRelationalModel.HashCodes](https://github.com/kudima03/Pure.Chart.RichRelationalModel.HashCodes) | Deterministic hash code implementations for chart rich relational model entities in the Pure ecosystem. |
| [Pure.Chart.RichRelationalModel.Abstractions.Serialization.System](https://github.com/kudima03/Pure.Chart.RichRelationalModel.Abstractions.Serialization.System) | System.Text.Json converters for the Pure.Chart rich relational model abstractions — IChartRichRelationalModel and related interfaces. |
| [Pure.Chart.RichRelationalModel.EFCore](https://github.com/kudima03/Pure.Chart.RichRelationalModel.EFCore) | EF Core DbContext for the Pure.Chart RichRelationalModel — maps chart, axis, chart type, and series entities to a relational database. |
| [Pure.Chart.RichRelationalModel.EFCore.Models](https://github.com/kudima03/Pure.Chart.RichRelationalModel.EFCore.Models) | EF Core entity record implementations of the chart rich relational model for the Pure ecosystem. |
| [Pure.Chart.RichRelationalModel.EFCore.Models.Configurations](https://github.com/kudima03/Pure.Chart.RichRelationalModel.EFCore.Models.Configurations) | EF Core IEntityTypeConfiguration\<T\> implementations for the Pure.Chart rich relational model — chart, axis, chart type, and series entity configurations. |

### Diagram Model

| Repository | Description |
|---|---|
| [Pure.Diagram.Model.Abstractions](https://github.com/kudima03/Pure.Diagram.Model.Abstractions) | Diagram model interfaces for the Pure ecosystem — immutable, composable abstractions over IDiagram, IDiagramType, and IDiagramSeries; AOT-compatible. |
| [Pure.Diagram.Model](https://github.com/kudima03/Pure.Diagram.Model) | Concrete immutable record implementations of the diagram domain model for the Pure ecosystem — implements Pure.Diagram.Model.Abstractions contracts. |
| [Pure.Diagram.Model.HashCodes](https://github.com/kudima03/Pure.Diagram.Model.HashCodes) | Deterministic hash code implementations for diagram model abstractions in the Pure ecosystem. |
| [Pure.Diagram.RelationalModel.Abstractions](https://github.com/kudima03/Pure.Diagram.RelationalModel.Abstractions) | Relational-model interfaces for diagram entities in the Pure ecosystem — immutable contracts for diagrams, diagram types, and series. |
| [Pure.Diagram.RelationalModel](https://github.com/kudima03/Pure.Diagram.RelationalModel) | Concrete relational model records for the Pure ecosystem — immutable implementations of diagram domain entities. |
| [Pure.Diagram.RelationalModel.HashCodes](https://github.com/kudima03/Pure.Diagram.RelationalModel.HashCodes) | Deterministic hash code implementations for diagram relational model entities in the Pure ecosystem. |
| [Pure.Diagram.RelationalModel.Abstractions.Serialization.System](https://github.com/kudima03/Pure.Diagram.RelationalModel.Abstractions.Serialization.System) | System.Text.Json converters for diagram relational model abstractions in the Pure ecosystem. |
| [Pure.Diagram.RichRelationalModel.Abstractions](https://github.com/kudima03/Pure.Diagram.RichRelationalModel.Abstractions) | Combined diagram domain-model and relational-model interfaces for the Pure ecosystem — rich view with both navigation properties and FK identity. |
| [Pure.Diagram.RichRelationalModel](https://github.com/kudima03/Pure.Diagram.RichRelationalModel) | Concrete immutable record implementations of the rich relational diagram model for the Pure ecosystem — carries both FK IDs and resolved navigations. |
| [Pure.Diagram.RichRelationalModel.HashCodes](https://github.com/kudima03/Pure.Diagram.RichRelationalModel.HashCodes) | Deterministic hash code implementations for diagram rich relational model entities in the Pure ecosystem. |
| [Pure.Diagram.RichRelationalModel.Abstractions.Serialization.System](https://github.com/kudima03/Pure.Diagram.RichRelationalModel.Abstractions.Serialization.System) | System.Text.Json converters for the Pure.Diagram rich relational model abstractions — IDiagramRichRelationalModel and related interfaces. |
| [Pure.Diagram.RichRelationalModel.EFCore](https://github.com/kudima03/Pure.Diagram.RichRelationalModel.EFCore) | EF Core DbContext for the Pure.Diagram RichRelationalModel — maps diagram, diagram type, and series entities to a relational database. |
| [Pure.Diagram.RichRelationalModel.EFCore.Models](https://github.com/kudima03/Pure.Diagram.RichRelationalModel.EFCore.Models) | EF Core entity record implementations of the diagram rich relational model for the Pure ecosystem. |
| [Pure.Diagram.RichRelationalModel.EFCore.Models.Configurations](https://github.com/kudima03/Pure.Diagram.RichRelationalModel.EFCore.Models.Configurations) | EF Core IEntityTypeConfiguration\<T\> implementations for the Pure.Diagram rich relational model — diagram, diagram type, and series entity configurations. |

### Infrastructure

| Repository | Description |
|---|---|
| [Pure.Template](https://github.com/kudima03/Pure.Template) | Project template for new Pure ecosystem NuGet libraries — pre-configured with standard CI workflows, code style, and package settings. |

---

*72 repositories · updated automatically via git submodules*
