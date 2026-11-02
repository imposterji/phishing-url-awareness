
# Phishing URL Awareness Checker – Test Results

## Test Environment
- Programming Language: Python
- Operating System: Windows
- Test Method: Manual testing
- Project Type: Text-based URL inspection

## Test Cases

| No. | Test Case | Sample URL | Actual Result | Status |
|---|---|---|---|---|
| 1 | Normal URL | https://www.example.com/login | No listed warning signs found | PASS |
| 2 | IP Address | http://192.0.2.10/account | IP address and HTTP warnings detected | PASS |
| 3 | Punycode | https://xn--example.invalid/ | Punycode warning detected | PASS |
| 4 | Many Subdomains | https://a.b.c.d.e.example.invalid/path | Many hostname segments/subdomains warning detected | PASS |
| 5 | @ Symbol | http://example.com@sample.invalid/login | @ symbol and HTTP warnings detected | PASS |
| 6 | Empty Input | Blank input | No URL entered | PASS |

## Additional Features Tested
- Continuous URL checking
- Warning summary
- Quit option using q
- Empty input handling 

## Conclusion

All five manual test cases produced the expected warning messages.

The program checks URL text only. It does not open URLs or guarantee that a website is safe.
