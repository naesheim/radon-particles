## Workload Node Type (Abstract)

Abstract node type representing a workload in general.

| Name | URI | Version | Derived From |
|:---- |:--- |:------- |:------------ |
| `Workload` | `radon.nodes.abstract.Workload` | 1.0.0 | `tosca.nodes.Root` |

### Properties

| Name | Required | Type | Constraint | Default Value | Description |
|:---- |:-------- |:---- |:---------- |:------------- |:----------- |
| `entries` | `false` | `radon.datatypes.workload.Entries` |   |   | Set of entries |

### Requirements

| Name | Capability Type | Node Type Constraint | Relationship Type | Occurrences |
|:---- |:--------------- |:-------------------- |:----------------- |:------------|
| `invoker` | `radon.capabilities.Invocable` |   | `radon.relationships.abstract.Triggers` | [0, UNBOUNDED] |
| `endpoint` | `tosca.capabilities.Endpoint` |   | `radon.relationships.abstract.ConnectsTo` | [0, UNBOUNDED] |
