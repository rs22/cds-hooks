# `observation-receive`

| Metadata | Value
| ---- | ----
| specificationVersion | 1.0
| hookVersion | 1.0
| hookMaturity | [0 - Draft](../../specification/1.0/#hook-maturity-model)

## Workflow

Any kind of patient observation is added to the system.

## Context

The patient for which a new observation was created.

Field | Optionality | Prefetch Token | Type | Description
----- | -------- | ---- | ---- | ----
`patientId` | REQUIRED | Yes | *string* | The FHIR `Patient.id` of the current patient in context
`observationId` | REQUIRED | Yes | *string* | The FHIR `Observation.id` of the added observation

### Examples


```json
"context":{
  "patientId" : "1288992",
  "observationId" : "1288992"
}
```


## Change Log

Version | Description
---- | ----
1.0 | Initial Release

