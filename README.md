![ChatGPT Image](ChatGPT%20Image%20May%2019,%202025,%2008_33_37%20PM.png)
Darknickon File Disclosure Scanner is a high-performance, multithreaded Java tool designed to detect and analyze sensitive file exposures across web archives. It leverages the Wayback Machine's CDX API to retrieve historical URLs, filters them based on file extensions indicative of sensitive data (e.g., .sql, .pdf, .docx, .zip), and assesses their accessibility. This tool is invaluable for penetration testers, bug bounty hunters, and security researchers aiming to uncover inadvertent file disclosures and misconfigurations.
![ChatGPT Result](ChatGPT%20Image%20May%2019,%202025,%2008_33_37%20PM.png)
🔍 Key Features
Wayback Machine Integration: Retrieves archived URLs for a specified domain using the CDX API.

Extension-Based Filtering: Targets URLs ending with potentially sensitive file extensions.

Multithreaded Scanning: Utilizes concurrent threads to efficiently check the availability of filtered URLs.

Status Code Evaluation: Identifies accessible files by analyzing HTTP response codes.

Automated Downloading: Optionally downloads accessible files of a specified extension for further analysis.

Customizable Parameters: Allows users to set thread count, timeout durations, and acceptable HTTP status codes.

📘 Usage
bash
Copy code
java -jar FileDisclosureScanner.jar -u <domain> [options]
Options:

-u <domain>: Target domain (required)

-o <output.txt>: Save results to specified file

--A <ext>: Download all files with the specified extension (e.g., pdf)

--threads <n>: Number of parallel threads (default: 12)

--timeout <ms>: HTTP timeout in milliseconds (default: 8000)

--status <codes>: Comma-separated list of acceptable HTTP status codes (default: 200,301,302,307,308,403)

-h, --help: Display help message

Examples:

bash
Copy code
java -jar FileDisclosureScanner.jar -u example.com
java -jar FileDisclosureScanner.jar -u example.com -o results.txt
java -jar FileDisclosureScanner.jar -u example.com --A pdf
🏷️ Suggested GitHub Tags for Enhanced Visibility
To maximize the discoverability of your project on GitHub, consider adding the following topics to your repository:

vulnerability-scanner

information-disclosure

file-scanner

security-tools

bugbounty

pentesting

wayback-machine

java-security

web-archive-analysis

sensitive-data-exposure

These tags align with common search terms used by the security community and will help position your tool alongside similar projects.

🚀 Promotion Strategy
GitHub Optimization:

Repository Description: Craft a concise and informative description highlighting the tool's purpose and capabilities.

README.md: Include detailed usage instructions, examples, and screenshots or GIFs demonstrating the tool in action.

Topics/Tags: Add the suggested GitHub topics to improve searchability.

Community Engagement:

Security Forums: Share your project on platforms like Reddit's r/netsec, r/bugbounty, and r/ethicalhacking.

Twitter/X: Announce releases and updates using relevant hashtags such as #BugBounty, #Infosec, and #OSINT.

Blog Posts and Tutorials:

Write articles detailing the tool's features, use cases, and real-world applications.

Create tutorials or walkthroughs demonstrating how to use the tool effectively.

Integration with Other Tools:

Explore integrating your scanner with other security tools or frameworks to enhance its functionality and reach.

📸 Visual Assets
To further promote your tool, consider creating visual assets such as:

Screenshots: Capture the tool's output and interface during scans.

Diagrams: Illustrate the scanning process and how the tool interacts with the Wayback Machine.

Demo Videos: Record short videos demonstrating the tool's setup and usage.

These assets can be included in your GitHub repository, shared on social media, and embedded in blog posts to provide a clearer understanding of the tool's capabilities.

By implementing these strategies, you'll enhance the visibility and adoption of your Darknickon File Disclosure Scanner within the security community. If you need assistance with any of these steps, feel free to ask!


Sources





