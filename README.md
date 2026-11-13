
# WSC Security Test

A collection of sample files and URLs for WedgeSecure Cloud QA, regression, and customer POC testing.

All test files contain synthetic data.

## Test Resources

### DLP & Text Extraction

Sample files are available in [dlp-tests](dlp-tests/).

| File | Purpose |
|---|---|
| `record.txt` | Keyword detection (CONFIDENTIAL) |
| `payment.txt` | Financial data detection using synthetic card numbers |
| `neutral.txt` | Negative control |
| `record.docx` | Word document text extraction |
| `record.pdf` | PDF text extraction |
| `bundle.zip` | Archive content extraction |

### URL Filtering

Test pages are available in [url-tests](url-tests/).

- [Allowed URL](url-tests/allowed.html)
- [Blocked URL](url-tests/blocked.html)

The actual allow/block result depends on the configured URL policy.

## How to Use

1. Open the [test website](https://wedgepsg.github.io/wsc-security-test/).
2. Select the test file or URL.
3. Configure the corresponding policy in WedgeIQ.
4. Verify detection or blocking in WedgeOS and WedgeIQ.

## Notes

- HTTPS inspection must be enabled when testing encrypted content.
- Document and archive scanning may require Text Extraction.
- This is a static website; file uploads require a separate endpoint.
- AAV and Web Filtering require appropriate test resources outside this repository.
