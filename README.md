# Hub import tests

Test files for importing into Camunda Hub through the import deep link:

```text
https://<hub-host>/import/resources?source=<url-encoded raw file URL>&title=<name>
```

Each folder holds one test case.

| Folder | Content |
|---|---|
| `mortgage-application-idp/` | Mortgage Blueprint project: a BPMN diagram, the IDP classification template, five IDP unstructured extraction templates (identity document, pay stub, bank statement, employment letter, property valuation), and a README |

To import several files at once, separate the encoded URLs in `source` with commas.
