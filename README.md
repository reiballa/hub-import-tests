# Hub import tests

Test files for importing into Camunda Hub through the import deep link:

```text
https://<hub-host>/import/resources?source=<url-encoded raw file URL>&title=<name>
```

Each folder holds one test case.

| Folder | Content |
|---|---|
| `mortgage-application-idp/` | Hub project download: a BPMN diagram that uses a published IDP classification template, the template file, and a README |
| `mortgage-application-idp/extraction-templates/` | Five IDP unstructured extraction templates for the mortgage Blueprint: identity document, pay stub, bank statement, employment letter, property valuation. Same provider settings as the classification template (pdfBox, Camunda-provided LLM) |

To import several files at once, separate the encoded URLs in `source` with commas.
