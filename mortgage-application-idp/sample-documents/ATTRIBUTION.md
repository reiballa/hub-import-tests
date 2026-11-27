# Sample documents

All documents are fictional and made for testing the Camunda mortgage application Blueprint. The
people, companies, accounts and properties don't exist.

The identity document embeds the specimen German identity card "Deutscher Personalausweis (2021
Version)" by the Bundesregierung der Bundesrepublik Deutschland, public domain under § 5 Abs. 1 UrhG,
from [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Deutscher_Personalausweis_(2021_Version).jpg).
Erika Mustermann is the fictional person the German government uses on specimen documents. The PDF
adds an invisible text layer with the card's data, like a scanned document after OCR, so the PDF
text extractor can read it.

| Folder | Expected outcome |
|---|---|
| `happy-path/` | Ready for underwriting, no user task |
| `needs-review/` | Review application with `INCOME_MISMATCH` and `NOT_PERMANENT` |
| `incomplete/` | Request missing documents asks for a bank statement |

Start each run with the values in `applicant.json`, including `checkDate`. `expected.json` lists the
expected document type and extracted values for every file.
