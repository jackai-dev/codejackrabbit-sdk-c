# CodeJackRabbit C API

<!-- omniwrap-api-reference eyJjb250cmFjdF9maW5nZXJwcmludCI6ImIwNjc4MWEyNmM0NDY5ZThmMTI4MzBhMDRkNDU1OTU3YmY2MjBkNDJiOWUxZGYxNTVlOTNlZTAwZjI5M2QxYzkiLCJvcGVyYXRpb25fY291bnQiOjI4LCJyZW5kZXJlciI6ImMiLCJ2ZXJzaW9uIjoiMS41LjAifQ -->

This generated index is tied to Semantic IR `1.14.0` and contract fingerprint `b06781a26c4469e8f12830a04d455957bf620d42b9e1df155e93ee00f293d1c9`. Every operation below is rendered from the same semantic contract and artifact-attested public member allocation as the SDK.

SDK maturity: **experimental**  
Artifact evidence: [`omniwrap-artifact.json`](omniwrap-artifact.json) binds this file by SHA-256 and is revalidated by the package gate.

## Shared types

- `AuditContextRequest`
- `AuditSnapshotsRequest`
- `ComplianceGateRequest`
- `DeveloperAuditRequest`
- `DeveloperEvidenceRequest`
- `FileChange`
- `FinOpsRequest`
- `ManagedDeveloperIdentity`
- `ManagedDeveloperIdentityRequest`
- `ReviewRequest`
- `WaitlistRequest`

## Resource `analysis`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9hbmFseXplX2NvbnRyYWN0X2RyaWZ0IiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6ImFuYWx5emVDb250cmFjdERyaWZ0IiwicGF0aCI6Ii92MS9hbmFseXNpcy9jb250cmFjdC1kcmlmdCIsInJlc291cmNlIjoiYW5hbHlzaXMiLCJzZWN0aW9uX3NoYTI1NiI6IjY1MGE4ZDVmNmE5ZDFkYWFhNGQ2NDgxMjg4ZjI5OWNlMjg4YjUxOTgxZWZhYTEyZTg1MDBmZmI3NzE5ZTU5MWUiLCJzaWduYXR1cmVfc2hhMjU2IjoiMjUzNjIxMDcyMTA4ZmE1OWE3ODIxZDU0MjFlMGY4ODA4MGRjZjA1MTlhMWMwMDUwZmUzM2JmODA1NjgyN2FhNSJ9 -->
### `client.omniwrap_analyze_contract_drift`

Operation ID: `analyzeContractDrift`  
Route: `POST` `/v1/analysis/contract-drift`  

#### Signature

```c
int omniwrap_analyze_contract_drift(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ReviewRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Contract drift report and SemVer recommendation | none |

#### Canonical required-input example

```json
{
  "body": {
    "files": [
      {
        "filename": "example"
      }
    ]
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJhbmFseXplQ29udHJhY3REcmlmdCJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9hbmFseXplX3BlcmZfZmluX29wcyIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJhbmFseXplUGVyZkZpbk9wcyIsInBhdGgiOiIvdjEvYW5hbHlzaXMvcGVyZi1maW5vcHMiLCJyZXNvdXJjZSI6ImFuYWx5c2lzIiwic2VjdGlvbl9zaGEyNTYiOiI0ZjRiZmM1ODljODI5NjVhNThkYmUwMWM4Y2RkMDY1M2RkNzUxNDlmMTU3MjRiZGNlM2ZjYzAyMmQyOGQxYTQ0Iiwic2lnbmF0dXJlX3NoYTI1NiI6IjEwYzY1ZDlhOGMwY2NlYjM5MWUxNDNhYWIyM2UzNzQ5ZGRjMzVmN2MzYjMzZmM2YzcwNzNkY2M1OWQyZWFlZjcifQ -->
### `client.omniwrap_analyze_perf_fin_ops`

Operation ID: `analyzePerfFinOps`  
Route: `POST` `/v1/analysis/perf-finops`  

#### Signature

```c
int omniwrap_analyze_perf_fin_ops(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ReviewRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Performance and FinOps audit report | none |

#### Canonical required-input example

```json
{
  "body": {
    "files": [
      {
        "filename": "example"
      }
    ]
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJhbmFseXplUGVyZkZpbk9wcyJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9wbGFuX3N0YWNrZWRfcHJfc3BsaXQiLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoicGxhblN0YWNrZWRQclNwbGl0IiwicGF0aCI6Ii92MS9hbmFseXNpcy9zcGxpdC1wciIsInJlc291cmNlIjoiYW5hbHlzaXMiLCJzZWN0aW9uX3NoYTI1NiI6ImY0NWNiYWFmMmYxMDBjYmZlYTM2ODQwYWQ0Y2EwMzMwNjY4NWQ2NmMyZjMxZTlkYWE3YmVlNTY1NjVjYzUwZGEiLCJzaWduYXR1cmVfc2hhMjU2IjoiZjA2NTY3YjYxOWVhZjdjNTZkOTk0MTIzMWZlZTMyZTI0MTcwOTRiMmJmYmJjYTZlMmYzOWY5ODRmMTBlMWIxOCJ9 -->
### `client.omniwrap_plan_stacked_pr_split`

Operation ID: `planStackedPrSplit`  
Route: `POST` `/v1/analysis/split-pr`  

#### Signature

```c
int omniwrap_plan_stacked_pr_split(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ReviewRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Ordered stacked PR plan and git commands | none |

#### Canonical required-input example

```json
{
  "body": {
    "files": [
      {
        "filename": "example"
      }
    ]
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJwbGFuU3RhY2tlZFByU3BsaXQifQ -->

## Resource `analytics`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9nZXRfYW5hbHl0aWNzX3JvaSIsIm1ldGhvZCI6IkdFVCIsIm9wZXJhdGlvbl9pZCI6ImdldEFuYWx5dGljc1JvaSIsInBhdGgiOiIvdjEvYW5hbHl0aWNzL3JvaSIsInJlc291cmNlIjoiYW5hbHl0aWNzIiwic2VjdGlvbl9zaGEyNTYiOiJkMmJkZTJiZWFkMmRkY2QwY2IyZjc3NjJlMjBjMTdmNWFlN2VhNGMxNjc2YTRjMWIyMTZmYzcyNDNkM2Q5OGFkIiwic2lnbmF0dXJlX3NoYTI1NiI6Ijk2ODI2MWM0MjlmY2Y3N2Q1YTc2N2ZiYjM5NDU1YjQ5MDFkYzBmNmQzNzgxNzJlN2Q4ZTQwYjhlYWVhMjRkOGYifQ -->
### `client.omniwrap_get_analytics_roi`

Operation ID: `getAnalyticsRoi`  
Route: `GET` `/v1/analytics/roi`  

#### Signature

```c
int omniwrap_get_analytics_roi(omniwrap_client_t *client, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | ROI telemetry summary | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRBbmFseXRpY3NSb2kifQ -->

## Resource `capabilities`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9nZXRfY2FwYWJpbGl0aWVzIiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoiZ2V0Q2FwYWJpbGl0aWVzIiwicGF0aCI6Ii92MS9jYXBhYmlsaXRpZXMiLCJyZXNvdXJjZSI6ImNhcGFiaWxpdGllcyIsInNlY3Rpb25fc2hhMjU2IjoiMGQ1YjZkOGRiZDFkYjk0NDk4MTExNzBjZjk2MmM1ZjUxYzk2NzdhNmNiNTZkZGY3MDdjMjNmZTRkMDVkNjNlZiIsInNpZ25hdHVyZV9zaGEyNTYiOiI1ZmEyYmU1YzMzYzBlMDY0NDUwZDI3ODI2YWEzNWEwZmM5MjMzZTdjMmViMzg0ZDZlNjZkM2U3OTM5YzIyN2QzIn0 -->
### `client.omniwrap_get_capabilities`

Operation ID: `getCapabilities`  
Route: `GET` `/v1/capabilities`  

#### Signature

```c
int omniwrap_get_capabilities(omniwrap_client_t *client, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Capabilities catalog | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRDYXBhYmlsaXRpZXMifQ -->

## Resource `compliance`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9ldmFsdWF0ZV9jb21wbGlhbmNlX2dhdGUiLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoiZXZhbHVhdGVDb21wbGlhbmNlR2F0ZSIsInBhdGgiOiIvdjEvY29tcGxpYW5jZS9nYXRlIiwicmVzb3VyY2UiOiJjb21wbGlhbmNlIiwic2VjdGlvbl9zaGEyNTYiOiI2MDU0NmE4Y2QxMzIzNDZhYjM2NGVmOWJlMmQ0NWU3NzdlMmU1NDY3ZWQ1ZjdhNDMzZmRkYmU2NzkyZjgzOWQ2Iiwic2lnbmF0dXJlX3NoYTI1NiI6ImUzMDc1NTFlZmEyNjhmZWI5N2YzYjI1YTQxZmRhMGQ0MDEyYjJmODdhNTMwMmY0NzJhYjFiYjA3OGE1NGI3Y2EifQ -->
### `client.omniwrap_evaluate_compliance_gate`

Operation ID: `evaluateComplianceGate`  
Route: `POST` `/v1/compliance/gate`  

#### Signature

```c
int omniwrap_evaluate_compliance_gate(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ComplianceGateRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Compliance gate verdict and SHA-256 attestation | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJldmFsdWF0ZUNvbXBsaWFuY2VHYXRlIn0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9leHBvcnRfc2FyaWYiLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoiZXhwb3J0U2FyaWYiLCJwYXRoIjoiL3YxL2NvbXBsaWFuY2Uvc2FyaWYiLCJyZXNvdXJjZSI6ImNvbXBsaWFuY2UiLCJzZWN0aW9uX3NoYTI1NiI6ImNhYzU2YjBlMjQwOTlkMWZlYjQ5MGNkYzBmOWFhOWU0OGVjNDBmNWIzNzczZmVkYTY5OTE5ZDQyZDMzNzI2ODMiLCJzaWduYXR1cmVfc2hhMjU2IjoiZTlkNmI1ZGYwYzlhZGRhMTQ4NDU4ZDY1ZDUyNTVhNGRhYjExMmFmNjZkZmEyYWU2MDdiNjdhYTg1ZWFjOWFjNiJ9 -->
### `client.omniwrap_export_sarif`

Operation ID: `exportSarif`  
Route: `POST` `/v1/compliance/sarif`  

#### Signature

```c
int omniwrap_export_sarif(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | SARIF 2.1.0 JSON document | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJleHBvcnRTYXJpZiJ9 -->

## Resource `developer_intelligence`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9jb2xsZWN0X2RldmVsb3Blcl9hdWRpdCIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJjb2xsZWN0RGV2ZWxvcGVyQXVkaXQiLCJwYXRoIjoiL2NsaS9tYW5hZ2VkL2RldmVsb3Blci1hdWRpdCIsInJlc291cmNlIjoiZGV2ZWxvcGVyX2ludGVsbGlnZW5jZSIsInNlY3Rpb25fc2hhMjU2IjoiOGYzYTdlODg1ZjJiNWNmM2Y3ZTAyOGI0NTU5MDM5ZjIxMzdmODA3NjBmMzAyZGU3YmQ0YTQ1MTJhMjg4NjA2MiIsInNpZ25hdHVyZV9zaGEyNTYiOiJkNjUwNGFkMGVjOTkxM2M4MWQ1MWM2OGM5YzM0ZDgwNWY1NGQ4NzdlMGVkNjhiMzBlOTZlZDUzYTEzMTY4N2I1In0 -->
### `client.omniwrap_collect_developer_audit`

Operation ID: `collectDeveloperAudit`  
Route: `POST` `/cli/managed/developer-audit`  

#### Signature

```c
int omniwrap_collect_developer_audit(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `DeveloperAuditRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Versioned report with source coverage, missing evidence and immutable snapshot reference. | application/json (object) |
| `default` | Explicit authentication, paid access, source authorization, capacity or collection blocker. | none |

#### Canonical required-input example

```json
{
  "body": {
    "from": "2026-01-09",
    "repositoryId": "1",
    "to": "2026-01-18"
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjb2xsZWN0RGV2ZWxvcGVyQXVkaXQifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9jdXJyZW50X2RldmVsb3Blcl9pZGVudGl0eSIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJjdXJyZW50RGV2ZWxvcGVySWRlbnRpdHkiLCJwYXRoIjoiL2NsaS9tYW5hZ2VkL2RldmVsb3Blci1pZGVudGl0eSIsInJlc291cmNlIjoiZGV2ZWxvcGVyX2ludGVsbGlnZW5jZSIsInNlY3Rpb25fc2hhMjU2IjoiNjQzMTE4NjBhZTNkYjgzMTc1NDYzNzc2NTEyOTExZjAyOTk4MWI3NDAzZjE5NjZlNjk2ZDNjYzhhMTcwMGFiMyIsInNpZ25hdHVyZV9zaGEyNTYiOiIyZDg0ZjAzNGE2NzI3NjE2OTVmM2Y0MmFjOWQ4NDM2ODg3MWE0ZjcxYjM0NDhjZjg1YzNlNDU3NTM3Yjk5NDk3In0 -->
### `client.omniwrap_current_developer_identity`

Operation ID: `currentDeveloperIdentity`  
Route: `POST` `/cli/managed/developer-identity`  

#### Signature

```c
int omniwrap_current_developer_identity(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ManagedDeveloperIdentityRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Current verified identity and authorized repositories. | application/json (ManagedDeveloperIdentity) |
| `default` | Explicit account, GitHub identity or source authorization blocker. | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjdXJyZW50RGV2ZWxvcGVySWRlbnRpdHkifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9kZWNsYXJlX2RldmVsb3Blcl9wcm9qZWN0X2NvbnRleHQiLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoiZGVjbGFyZURldmVsb3BlclByb2plY3RDb250ZXh0IiwicGF0aCI6Ii9jbGkvbWFuYWdlZC9hdWRpdC1jb250ZXh0IiwicmVzb3VyY2UiOiJkZXZlbG9wZXJfaW50ZWxsaWdlbmNlIiwic2VjdGlvbl9zaGEyNTYiOiI4YWEzMzZhMzFkZGQwZTk5MjUyNDcyZDVmYThkYjQ2NmMzNDNkZGE2NWJlMDJkYjc1ZTZjNTEzYmEwYmIwZmUwIiwic2lnbmF0dXJlX3NoYTI1NiI6IjI4MzVjYzgwNTEyMWNiZmEwZTE3YzU1MDYxMmI2YTUzMDU5ZGQ3ODU3YzQwN2RmYzYwOTE5N2M4MzE4MDgxODMifQ -->
### `client.omniwrap_declare_developer_project_context`

Operation ID: `declareDeveloperProjectContext`  
Route: `POST` `/cli/managed/audit-context`  

#### Signature

```c
int omniwrap_declare_developer_project_context(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `AuditContextRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Immutable declaration or correction receipt. | application/json (object) |
| `default` | Explicit authorization, contributor identity, correction or storage capacity blocker. | none |

#### Canonical required-input example

```json
{
  "body": {
    "declaration": {
      "contributorId": "1",
      "effectiveFrom": "2026-01-02",
      "effectiveTo": "2026-01-11",
      "snapshotId": "aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      "source": "example",
      "supersedes": "example",
      "type": "project_join",
      "value": "example"
    },
    "repositoryId": "1"
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJkZWNsYXJlRGV2ZWxvcGVyUHJvamVjdENvbnRleHQifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9tYW5hZ2VkX2F1ZGl0X3NuYXBzaG90cyIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJtYW5hZ2VkQXVkaXRTbmFwc2hvdHMiLCJwYXRoIjoiL2NsaS9tYW5hZ2VkL2F1ZGl0LXNuYXBzaG90cyIsInJlc291cmNlIjoiZGV2ZWxvcGVyX2ludGVsbGlnZW5jZSIsInNlY3Rpb25fc2hhMjU2IjoiMDRiODExMTE2NTEyMmFjODkyNjhmZTQ2YjVmODVkZjJhNDkxMjUzYjE0MGM3NDc2ZjY1ZTcwNjMyMDVkOTRlZiIsInNpZ25hdHVyZV9zaGEyNTYiOiI5NTZkNjliNGFiOWM2YmVhMmJkMDdkOTE5NWZmZjI1ZTUyODEyYjFlYjc3Y2FmYzE3NzQwMjAyZmY5ZTYzY2MyIn0 -->
### `client.omniwrap_managed_audit_snapshots`

Operation ID: `managedAuditSnapshots`  
Route: `POST` `/cli/managed/audit-snapshots`  

#### Signature

```c
int omniwrap_managed_audit_snapshots(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `AuditSnapshotsRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Snapshot list or digest-verified immutable envelope. | application/json (object) |
| `default` | Explicit authorization, expiry, missing snapshot or integrity blocker. | none |

#### Canonical required-input example

```json
{
  "body": {
    "action": "list",
    "repositoryId": "1"
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJtYW5hZ2VkQXVkaXRTbmFwc2hvdHMifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9wcm92aWRlcl9jb3N0X2V2aWRlbmNlIiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6InByb3ZpZGVyQ29zdEV2aWRlbmNlIiwicGF0aCI6Ii9jbGkvbWFuYWdlZC9maW5vcHMiLCJyZXNvdXJjZSI6ImRldmVsb3Blcl9pbnRlbGxpZ2VuY2UiLCJzZWN0aW9uX3NoYTI1NiI6IjA1MDA2MGYzNDUwZGM3OWM0MzZkMDMxNjEwNjRhOTAzY2JhOWJlYzE2NTRiYmQ1MTA1N2EyZThiZjlmYzgzZDUiLCJzaWduYXR1cmVfc2hhMjU2IjoiN2FkNDdkNWRjZTUyMzhmMjlmMzliYWY5YWM1MmQyMTM4NzM5NGJkZTNiOWRjNDQ0MzQ4OWZlMmZlMTA3ZTZmZCJ9 -->
### `client.omniwrap_provider_cost_evidence`

Operation ID: `providerCostEvidence`  
Route: `POST` `/cli/managed/finops`  

#### Signature

```c
int omniwrap_provider_cost_evidence(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `FinOpsRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Server report or declaration receipt. Unknown costs remain null. | application/json (object) |
| `default` | Explicit permission, paid access, source or declaration validation blocker. | none |

#### Canonical required-input example

```json
{
  "body": {
    "action": "report"
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJwcm92aWRlckNvc3RFdmlkZW5jZSJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9zdWJtaXRfZGV2ZWxvcGVyX2V2aWRlbmNlIiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6InN1Ym1pdERldmVsb3BlckV2aWRlbmNlIiwicGF0aCI6Ii9jbGkvbWFuYWdlZC9kZXZlbG9wZXItZXZpZGVuY2UiLCJyZXNvdXJjZSI6ImRldmVsb3Blcl9pbnRlbGxpZ2VuY2UiLCJzZWN0aW9uX3NoYTI1NiI6IjEwN2JlNjBlMDVlZGUxMWIwNjc2ZTk5ZGQ1MTc2NjEyMTM5OGIxMTkyZjkwNDcwOTdjYmIxYmFmZjJkNDY4ZWMiLCJzaWduYXR1cmVfc2hhMjU2IjoiNjI4N2JiMzIxZWUwODkzOGMzODVmYWNhOWE5MWQ4ZjAyMDMxZjdjZmQzNTJkMDdiNmIwZWQ0YWUxMWE1NTAyZiJ9 -->
### `client.omniwrap_submit_developer_evidence`

Operation ID: `submitDeveloperEvidence`  
Route: `POST` `/cli/managed/developer-evidence`  

#### Signature

```c
int omniwrap_submit_developer_evidence(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `DeveloperEvidenceRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Accepted and duplicate span counts. | application/json (object) |
| `default` | Explicit identity, repository, paid access or evidence validation blocker. | none |

#### Canonical required-input example

```json
{
  "body": {
    "category": "coding",
    "input": {},
    "repositoryId": "1"
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJzdWJtaXREZXZlbG9wZXJFdmlkZW5jZSJ9 -->

## Resource `health`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9nZXRfaGVhbHRoIiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoiZ2V0SGVhbHRoIiwicGF0aCI6Ii9oZWFsdGgiLCJyZXNvdXJjZSI6ImhlYWx0aCIsInNlY3Rpb25fc2hhMjU2IjoiMmM0ZGEyNGU3ODc2YTBmYmQ4MmFiZWFiMTFkZmEzZjM0ZjU2NDk2MzRkMjlmMThiYjQwNmRhYTU0YThhODgwNiIsInNpZ25hdHVyZV9zaGEyNTYiOiIyYWM5YjkwNDk0NjBiYWY1ZWJlODVjNDgzOWYyNTQ1ZDIxNzU2NTMyODFlODEzN2ViZTVmMzc2ZWI1ZDMwZDUxIn0 -->
### `client.omniwrap_get_health`

Operation ID: `getHealth`  
Route: `GET` `/health`  

#### Signature

```c
int omniwrap_get_health(omniwrap_client_t *client, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Server health status | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRIZWFsdGgifQ -->

## Resource `reviews`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9idWlsZF9hdXRvZml4X2J1bmRsZSIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJidWlsZEF1dG9maXhCdW5kbGUiLCJwYXRoIjoiL3YxL3Jldmlld3MvYXV0b2ZpeCIsInJlc291cmNlIjoicmV2aWV3cyIsInNlY3Rpb25fc2hhMjU2IjoiOGM0YTc0NTNlYzBiMGRhYjQxOWUyNzJlNjJkNzY2M2EzOThkMWQwMzRjNzAxNWM5YmFhMmM0YzQ5N2E0NDEyNiIsInNpZ25hdHVyZV9zaGEyNTYiOiIxOWI0YTdhN2YxZjM0MDU5NTg1YTZlZTA3Y2JlYjZkMmMwZWY3MjQ5YzkwMGNiMjE5YmM0MjUxYTY3YTc5MjIyIn0 -->
### `client.omniwrap_build_autofix_bundle`

Operation ID: `buildAutofixBundle`  
Route: `POST` `/v1/reviews/autofix`  

#### Signature

```c
int omniwrap_build_autofix_bundle(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ReviewRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Remediation patch bundle | none |

#### Canonical required-input example

```json
{
  "body": {
    "files": [
      {
        "filename": "example"
      }
    ]
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJidWlsZEF1dG9maXhCdW5kbGUifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9jb21wdXRlX3Jpc2tfcmFkYXIiLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoiY29tcHV0ZVJpc2tSYWRhciIsInBhdGgiOiIvdjEvcmV2aWV3cy9yaXNrLXJhZGFyIiwicmVzb3VyY2UiOiJyZXZpZXdzIiwic2VjdGlvbl9zaGEyNTYiOiJmNjYwYTg2MjZiYTc1OTUyNTQ0NjFkODc5NmQ4MDFhNzFiNjQ3NTQ1M2RjNjE0MmYxNTMxZDAxNTBjMjk3ODg1Iiwic2lnbmF0dXJlX3NoYTI1NiI6Ijk1MjA0OTI3NGMxMThjMDI5NjhlZjYzNTY3YTJlYTVmYWJjODYyMWZkZTA0OWE2YTliOWRmZTk0M2IzYjFiZmQifQ -->
### `client.omniwrap_compute_risk_radar`

Operation ID: `computeRiskRadar`  
Route: `POST` `/v1/reviews/risk-radar`  

#### Signature

```c
int omniwrap_compute_risk_radar(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ReviewRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | 6-axis Risk Radar telemetry | none |

#### Canonical required-input example

```json
{
  "body": {
    "files": [
      {
        "filename": "example"
      }
    ]
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjb21wdXRlUmlza1JhZGFyIn0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9jcmVhdGVfcmV2aWV3IiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6ImNyZWF0ZVJldmlldyIsInBhdGgiOiIvdjEvcmV2aWV3cyIsInJlc291cmNlIjoicmV2aWV3cyIsInNlY3Rpb25fc2hhMjU2IjoiODI3NzI0NGY3MzFlNTZmNjk5ZWVjODZjODU2ZjQzZGRiMWU2NDY2MDU2YTdlOTNkNTQ4NjVhMjNlZmNmMDBmMiIsInNpZ25hdHVyZV9zaGEyNTYiOiI3ZTllZWRjYjRmNDUxMjJkN2VkZjE5ZGEyNDUyNDRmOGZiZGM2MWJhNTcxMzIxZjM5MzJmMTEyNjU4N2M5YTQxIn0 -->
### `client.omniwrap_create_review`

Operation ID: `createReview`  
Route: `POST` `/v1/reviews`  

#### Signature

```c
int omniwrap_create_review(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ReviewRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Completed review result with findings, blast radius, and change stack | none |

#### Canonical required-input example

```json
{
  "body": {
    "files": [
      {
        "filename": "example"
      }
    ]
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjcmVhdGVSZXZpZXcifQ -->

## Resource `saas`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9maW5hbGl6ZV9tZXRlcmluZ19xdW90YSIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJmaW5hbGl6ZU1ldGVyaW5nUXVvdGEiLCJwYXRoIjoiL3YxL3NhYXMvbWV0ZXJpbmcvZmluYWxpemUiLCJyZXNvdXJjZSI6InNhYXMiLCJzZWN0aW9uX3NoYTI1NiI6ImU3ZTgxYTVlODJmN2M3Zjc5NjZhNTFiNjg3YzMzZjRkODhlOTVjY2FmMDBiNGU1NTc4NTYyOGQzMGE0MzE0ZDkiLCJzaWduYXR1cmVfc2hhMjU2IjoiNDNhMGQ3ZDM4N2FjMjdmMTA2Y2Q4N2FlZTJhMzRkZGVhMzc0YjI4ZTZiZjNkZTk1MTBlZTYyOThkY2JmNmQzYyJ9 -->
### `client.omniwrap_finalize_metering_quota`

Operation ID: `finalizeMeteringQuota`  
Route: `POST` `/v1/saas/metering/finalize`  

#### Signature

```c
int omniwrap_finalize_metering_quota(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Finalized metering settlement | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJmaW5hbGl6ZU1ldGVyaW5nUXVvdGEifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9nZXRfc2Fhc19ibHVlcHJpbnQiLCJtZXRob2QiOiJHRVQiLCJvcGVyYXRpb25faWQiOiJnZXRTYWFzQmx1ZXByaW50IiwicGF0aCI6Ii92MS9zYWFzL2JsdWVwcmludCIsInJlc291cmNlIjoic2FhcyIsInNlY3Rpb25fc2hhMjU2IjoiYjI5MzU5NzY1MmIxMjM1YWMwZWFhOWEyMTgyNTk5MGFlOGI2NTcwMjFiMDZkZDA5MDk1NTA2NGEzZTc0MDY3YyIsInNpZ25hdHVyZV9zaGEyNTYiOiI4YTE2ZmJmMTljYWViYmNhZDc0ZTBiOWQyZmM3YTk2ZGY4M2RlMWUyYzA5ODRjZDI0NmYwMDk2M2EwZjk2NWQ5In0 -->
### `client.omniwrap_get_saas_blueprint`

Operation ID: `getSaasBlueprint`  
Route: `GET` `/v1/saas/blueprint`  

#### Signature

```c
int omniwrap_get_saas_blueprint(omniwrap_client_t *client, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Autonomous SaaS blueprint | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRTYWFzQmx1ZXByaW50In0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9pc3N1ZV9zdXJmYWNlX2xlYXNlIiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6Imlzc3VlU3VyZmFjZUxlYXNlIiwicGF0aCI6Ii92MS9zYWFzL3N1cmZhY2UtbGVhc2UvaXNzdWUiLCJyZXNvdXJjZSI6InNhYXMiLCJzZWN0aW9uX3NoYTI1NiI6IjU5MTRjZjFhY2RhMjJlZjg3NzVmYmVjNTJhZjc2ZGRiNzkxMTk0Y2NlNmM4ZmJlYjFhZjdhZGFkMWI1YzIwOWMiLCJzaWduYXR1cmVfc2hhMjU2IjoiMWE0Mjc0MTRlNGRkZjY5ZDJkNjU0ZDBhMGU3MDVmMjk5OTNiNmM3NTRiMDU4YjFmY2M4MWUyMTk5NzhjNDJiMiJ9 -->
### `client.omniwrap_issue_surface_lease`

Operation ID: `issueSurfaceLease`  
Route: `POST` `/v1/saas/surface-lease/issue`  

#### Signature

```c
int omniwrap_issue_surface_lease(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Issued surface lease token | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJpc3N1ZVN1cmZhY2VMZWFzZSJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9yZXNlcnZlX21ldGVyaW5nX3F1b3RhIiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6InJlc2VydmVNZXRlcmluZ1F1b3RhIiwicGF0aCI6Ii92MS9zYWFzL21ldGVyaW5nL3Jlc2VydmUiLCJyZXNvdXJjZSI6InNhYXMiLCJzZWN0aW9uX3NoYTI1NiI6ImQzNDAxZjYzZDZiMTQxYjk3ZGI3YjUwZmVjZTRlZTA3ZTY3M2E4NDRkNjFhOWNmNzNlOTc5YjM5NmY0NjExYzUiLCJzaWduYXR1cmVfc2hhMjU2IjoiZDc1NWQ4NTc4MzJiM2Y1Njk0MGJmYzYzNmFkZDFkNGI2NTg0MDQzM2QyOThjNGRmYmU2OWQ5ZmU5NjExZGIzNSJ9 -->
### `client.omniwrap_reserve_metering_quota`

Operation ID: `reserveMeteringQuota`  
Route: `POST` `/v1/saas/metering/reserve`  

#### Signature

```c
int omniwrap_reserve_metering_quota(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Metering reservation record | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJyZXNlcnZlTWV0ZXJpbmdRdW90YSJ9 -->

## Resource `sbom`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9nZW5lcmF0ZV9zYm9tIiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6ImdlbmVyYXRlU2JvbSIsInBhdGgiOiIvdjEvc2JvbSIsInJlc291cmNlIjoic2JvbSIsInNlY3Rpb25fc2hhMjU2IjoiY2UxODI3MDUxY2VhYTBmMWE2YmMxMjViNzI2YWY1OTAxZTUyODE3NjhmZTBiM2RhNWI0OThlMTFiYTU1YTNlYSIsInNpZ25hdHVyZV9zaGEyNTYiOiJhNTMyMzFkNTUzNDM3NDNlODgxOTFiMTk0Njc0MmE4OGYzNmNjMzUzYjUzZjNmZGI0M2VmYTM5MGY0MmY4NTk1In0 -->
### `client.omniwrap_generate_sbom`

Operation ID: `generateSbom`  
Route: `POST` `/v1/sbom`  

#### Signature

```c
int omniwrap_generate_sbom(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ReviewRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | CycloneDX 1.5 SBOM JSON | none |

#### Canonical required-input example

```json
{
  "body": {
    "files": [
      {
        "filename": "example"
      }
    ]
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZW5lcmF0ZVNib20ifQ -->

## Resource `supply_chain`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9hbmFseXplX3N1cHBseV9jaGFpbiIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJhbmFseXplU3VwcGx5Q2hhaW4iLCJwYXRoIjoiL3YxL3N1cHBseS1jaGFpbi9hbmFseXplIiwicmVzb3VyY2UiOiJzdXBwbHlfY2hhaW4iLCJzZWN0aW9uX3NoYTI1NiI6IjE0ZTQ0Y2U5ZGE3MGYzOTYzOTJmNTc1MDY5Y2IxMWRjY2ZjZTJkMDZlMmY4NTI5NDFjZWI0MzM0NzI3MjA3MjIiLCJzaWduYXR1cmVfc2hhMjU2IjoiYzU4NTliMDdhZDQ0M2Q2NmJlYzM4NjQ3N2JhNWQyM2QzZWM1ZGQ1MjljNzdiMWEyMmZlNTUxMjg5MTdhZDExYiJ9 -->
### `client.omniwrap_analyze_supply_chain`

Operation ID: `analyzeSupplyChain`  
Route: `POST` `/v1/supply-chain/analyze`  

#### Signature

```c
int omniwrap_analyze_supply_chain(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ReviewRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Supply-chain security audit | none |

#### Canonical required-input example

```json
{
  "body": {
    "files": [
      {
        "filename": "example"
      }
    ]
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJhbmFseXplU3VwcGx5Q2hhaW4ifQ -->

## Resource `tasks`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9jcmVhdGVfY29kaW5nX3Rhc2siLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoiY3JlYXRlQ29kaW5nVGFzayIsInBhdGgiOiIvdjEvdGFza3MiLCJyZXNvdXJjZSI6InRhc2tzIiwic2VjdGlvbl9zaGEyNTYiOiJkNjVlNzE1ZDI0MGQxMmFjYmZmZDM4NzZkNjlmOWVkMjc3YTE3YjkxMzIzZDU2OGYyNTE2YTQwZGM4YWM1NTY4Iiwic2lnbmF0dXJlX3NoYTI1NiI6IjBjNmE4OTM4ODU5ZDczMTYwZmNlZjYxNWQ0M2JlODkyYzI1NDIxMTI1YTkxMzA2MzVjNDNiMzBlOGM5ODkxZWUifQ -->
### `client.omniwrap_create_coding_task`

Operation ID: `createCodingTask`  
Route: `POST` `/v1/tasks`  

#### Signature

```c
int omniwrap_create_coding_task(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `201` | Created coding task | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjcmVhdGVDb2RpbmdUYXNrIn0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9saXN0X2NvZGluZ190YXNrcyIsIm1ldGhvZCI6IkdFVCIsIm9wZXJhdGlvbl9pZCI6Imxpc3RDb2RpbmdUYXNrcyIsInBhdGgiOiIvdjEvdGFza3MiLCJyZXNvdXJjZSI6InRhc2tzIiwic2VjdGlvbl9zaGEyNTYiOiJlNjJhM2VjMmUwNWJiMTEyZmYyM2M0OGFlNWNiYjZiYTFjMTAzYzkxMmNkMzdkYzlmMzg1NmQ2YjQxOTA3MmFhIiwic2lnbmF0dXJlX3NoYTI1NiI6Ijc2Yzk3MmVjYzlkNzA5NTlmNmEwOTYxOGMwZTU5YjJmZDYzOWNhN2Y1YzNkNDU5NmQ5YjNmNmU1NzkyYzRjMjMifQ -->
### `client.omniwrap_list_coding_tasks`

Operation ID: `listCodingTasks`  
Route: `GET` `/v1/tasks`  

#### Signature

```c
int omniwrap_list_coding_tasks(omniwrap_client_t *client, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Task list | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJsaXN0Q29kaW5nVGFza3MifQ -->

## Resource `triage`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9nZXRfdHJpYWdlX3F1ZXVlIiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoiZ2V0VHJpYWdlUXVldWUiLCJwYXRoIjoiL3YxL3RyaWFnZSIsInJlc291cmNlIjoidHJpYWdlIiwic2VjdGlvbl9zaGEyNTYiOiIzYjRkZmE0M2UzNGQ1MWM0YTRhODJjYmQ5NzBlYTZiYzk3ZDRiZThhMjMzNjA3NGEzNDRkNTAxODFlYjdjNjA1Iiwic2lnbmF0dXJlX3NoYTI1NiI6IjI5MThhZjgwYzkxZjMyY2RjMGU2YjE5NjUwZDA5ZTQyMmE4NTViOWQ0ZWQwNzViMmE2ZDViNzJjNmIzOWM5ZjAifQ -->
### `client.omniwrap_get_triage_queue`

Operation ID: `getTriageQueue`  
Route: `GET` `/v1/triage`  

#### Signature

```c
int omniwrap_get_triage_queue(omniwrap_client_t *client, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Triaged PR queue | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRUcmlhZ2VRdWV1ZSJ9 -->

## Resource `waitlist`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9saXN0X3dhaXRsaXN0IiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoibGlzdFdhaXRsaXN0IiwicGF0aCI6Ii92MS93YWl0bGlzdCIsInJlc291cmNlIjoid2FpdGxpc3QiLCJzZWN0aW9uX3NoYTI1NiI6IjUwMmRhOGFmMGYyYWYwN2MyYWJkMDRkZmIwYjFkNGE4Yjk5YTQ3NzYwOGRmNGEwNzUzNDgzMDNmYzNhOWRlNDYiLCJzaWduYXR1cmVfc2hhMjU2IjoiZmYyOTE3M2YwOTg3N2NhNzM5M2ZjN2UzMTRmN2QwN2Y2ZGY1NzVjN2Q4ZDE2ODhlZTE3ZmQ0NTA5NTlmNTFiYSJ9 -->
### `client.omniwrap_list_waitlist`

Operation ID: `listWaitlist`  
Route: `GET` `/v1/waitlist`  

#### Signature

```c
int omniwrap_list_waitlist(omniwrap_client_t *client, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Waitlist entries | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJsaXN0V2FpdGxpc3QifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvbW5pd3JhcF9yZWdpc3Rlcl93YWl0bGlzdCIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJyZWdpc3RlcldhaXRsaXN0IiwicGF0aCI6Ii92MS93YWl0bGlzdCIsInJlc291cmNlIjoid2FpdGxpc3QiLCJzZWN0aW9uX3NoYTI1NiI6IjcwMTI1ZDRlMDJhZDliZDg5NWJjMDAyZDM2NTJlOGQ0OGI2M2JhODFhYjYzMzEwZTRlYWI0YmIyNjk5NmM3MDQiLCJzaWduYXR1cmVfc2hhMjU2IjoiYmQ0MzdkNjRjMmU3NmVkYmE3YjY3NGU4NDgxNzE2ODRhNjcwOTA1MTFkZDZkOGU4YTc2OTdiMGI2NmRhOWRjNiJ9 -->
### `client.omniwrap_register_waitlist`

Operation ID: `registerWaitlist`  
Route: `POST` `/v1/waitlist`  

#### Signature

```c
int omniwrap_register_waitlist(omniwrap_client_t *client, const char *body_json, omniwrap_response_t *out_response)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `WaitlistRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `201` | Waitlist entry created | none |

#### Canonical required-input example

```json
{
  "body": {
    "email": "example-c65f@example.test"
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJyZWdpc3RlcldhaXRsaXN0In0 -->

