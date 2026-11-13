
# WSC Security Test
Sample files for testing WedgeSecure Cloud security features, including DLP, Keyword Detection, Text Extraction, and URL Filtering.

All files contain synthetic test data for QA and customer POC testing.

## Test Files
| File | Purpose |
|---|---|
| `record.txt` | Keyword detection (CONFIDENTIAL) |
| `payment.txt` | Financial data detection using test card numbers |
| `neutral.txt` | Negative test with normal content |
| `record.docx` | Keyword detection in Word documents |
| `record.pdf` | Keyword detection in PDF documents |
| `bundle.zip` | Keyword detection inside compressed files |

## How to Use
1. Open or download files from the [test website](https://wedgepsg.github.io/wsc-security-test/).
2. Configure the relevant security policy in WedgeIQ.
3. Verify detection or blocking events in WedgeOS and WedgeIQ.

## Notes
- Document and ZIP content inspection may require Text Extraction.
- HTTPS inspection must be enabled when testing encrypted traffic.
- This site provides downloadable test files only. File uploads require a separate test endpoint.
- Actual detection depends on the configured policies and enabled security features.
