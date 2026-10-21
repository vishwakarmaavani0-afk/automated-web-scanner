README File
Automated Web Scanner (HTTP Security Headers &
CORS)
**Author:** Avani Vishwakarma
**Course:** BCA
**Institution:** SMS Lucknow
Project overview
A beginner-friendly Python utility that sends a single HTTP GET request to a website and checks for selected
HTTP security headers and the `Access-Control-Allow-Origin` CORS response header. Findings are printed in
the terminal and saved to `scan_report.txt`.
Features
• Adds `https://` when the URL has no scheme.
• Checks five headers: HSTS, CSP, X-Frame-Options, X-Content-Type-Options and Referrer-Policy.
• Reports whether the CORS response header is present and flags a wildcard (`*`) for review.
• Handles timeouts, TLS errors and other request errors.
• Exports findings to a text report.
Requirements
• Python 3.9 or newer (recommended)
• Internet connection
• `requests` library
Setup and run
1. Download or clone the repository
git clone https://github.com/YOUR-USERNAME/automated-web-scanner.git
cd automated-web-scanner
2. Install dependencies
python -m pip install -r requirements.txt
3. Run the scanner
python web_scanner.py
When prompted, enter a domain such as `example.com` or a full URL such as `https://example.com`.
4. View the report
After the scan, open `scan_report.txt` in the same folder.Project structure
automated-web-scanner/
■■■ web_scanner.py
■■■ requirements.txt
■■■ README.md
■■■ Project_Report.pdf
■■■ .gitignore
`scan_report.txt` is generated when the program runs and is intentionally excluded from Git by default.
Important limitations
• This is a basic educational checker, not a full penetration-testing tool.
• A missing header does not automatically prove a website is vulnerable.
• A wildcard CORS header needs context; it is not always a vulnerability.
• Results depend on the target's current response and may vary over time.
• The scanner checks response headers only; it does not crawl pages or test application logic.
Responsible use
Only scan websites you own or have explicit permission to assess. Keep requests low-volume and respect the
site's terms and policies. Do not use this project to disrupt services or access data without authorization.
Author
Avani Vishwakarma | BCA | SMS Lucknow
