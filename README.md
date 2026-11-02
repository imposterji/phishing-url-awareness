
# EWB – Phishing URL Awareness Checker

A beginner-friendly Python cybersecurity project that inspects URL text for common phishing warning signs.

## Project Overview

Phishing attacks use deceptive links to trick users into sharing sensitive information such as passwords, banking details, and personal data.

This project helps users identify suspicious URL characteristics through simple text-based checks.

**Important:** This tool does not open URLs, visit websites, or guarantee that a URL is safe.

## Features

- Detects IP addresses used as hostnames.
- Identifies suspicious use of the @ symbol.
- Detects HTTP URLs.
- Identifies punycode-style hostnames.
- Detects URLs with many hostname segments.
- Provides warning summaries.
- Supports continuous URL checking.
- Allows users to exit using q.

## Technologies Used

- Python 3.13.11
- Python standard library
- Visual Studio Code

## Project Structure

phishing-url-awareness/
│
├── phishing_checker.py
├── README.md
├── requirements.txt
├── tests/
│   └── test_samples.md
└── screenshots/
    ├── sample_run.png
    └── test_results.png

## Installation and Execution

1. Install Python 3.
2. Clone or download this repository.
3. Open the project directory in a terminal.
4. Run:

```bash
python phishing_checker.py
```

5. Enter a URL when prompted.
6. Type q to exit.

## Sample Output

```text
Enter a sample URL:

Result:
- Uses an IP address instead of a familiar domain.
- Uses HTTP. HTTPS alone does not prove trust.

REVIEW CAREFULLY: 2 warning sign(s) found.
```

## Testing

Five manual test cases were completed:

1. Normal URL
2. IP address
3. Punycode hostname
4. Multiple subdomains
5. @ symbol

See [test_samples.md](tests/test_samples.md) for the test results.

## Limitations

- Does not perform live website analysis.
- Does not check website reputation or domain age.
- Does not inspect website content.
- Cannot guarantee that a URL is safe.
- Warning signs are indicators for further inspection, not proof of phishing.

## Future Improvements

- Integrate threat intelligence APIs.
- Add domain reputation checks.
- Build a web-based user interface.
- Add URL analysis reports.
- Integrate security monitoring tools.

## Ethical Use

This project is developed for cybersecurity awareness and educational purposes.

## Author

Developed as part of the EWB Phishing URL Awareness Checker project.
