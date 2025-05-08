# Dark Web Project

## Objective

This project aimed to develop a system for automating the monitoring and analysis of dark web marketplaces using Tor-based scraping tools. The goal was to identify cyber threats such as stolen credentials, malware, and illicit services. By applying web scraping, Natural Language Processing (NLP), and data visualization, the system would produce actionable threat intelligence insights despite the challenges of unstructured and volatile data sources.
### Skills Learned

- Configured Tor and Privoxy proxies to securely access .onion sites

- Gained experience using Scrapy, Requests, and BeautifulSoup for web scraping

- Parsed and cleaned inconsistent HTML structures from dark web marketplaces

- Developed Python scripts for classifying, extracting, and visualizing data

- Applied regex for pricing analysis and called HaveIBeenPwned API for breach checks

- Created simulated threat intelligence reports with visualized trends

- Strengthened problem-solving skills in a real-world data gathering context

### Tools Used
Tor & Privoxy – Anonymous access to hidden services

Scrapy / Requests / BeautifulSoup4 – Web scraping frameworks

Python (Pandas, Regex, Seaborn) – Data processing and visualization

HaveIBeenPwned API – Breach verification of compromised credentials

Ahmia.fi – Search engine for locating active .onion marketplaces


## Steps
Milestone 1 – Tor + Scrapy Setup
Installed Tor Browser and configured the torrc file to enable SOCKS5 proxy routing through port 9050. Verified Tor’s operation using netstat and curl commands. Installed Scrapy and built a basic spider configured to route traffic through Tor. Successfully confirmed that Scrapy could extract content from a test .onion site.

Milestone 2 – Dark Web Marketplace Discovery
Used Ahmia.fi to research and verify active .onion marketplaces. Categorized each by illicit service type (e.g., credentials, malware, drugs, weapons). Documented marketplace names, access requirements, and the type of data offered. Built a vetted target list for future scraping.

Milestone 3 – Scraping & HTML Extraction
Faced technical setbacks with Scrapy spiders not resolving .onion addresses due to DNS issues. Switched to using Python’s requests with Tor proxy and BeautifulSoup to parse HTML. Successfully extracted data manually from saved pages, including product names, prices, and vendor info.

Milestone 4 – Data Analysis & Breach Correlation
Attempted structured parsing of scraped HTML files using BeautifulSoup and Pandas. Implemented regex to detect pricing and developed tagging logic to classify data (SSNs, credentials, malware). Called HaveIBeenPwned API to test for known breaches, although most listings lacked clean email formats. Faced challenges due to inconsistent formatting.

Milestone 5 – Final Threat Intelligence Report
Compiled a simulated cyber threat intelligence report using cleaned and categorized data from verified marketplaces. Built visual charts to show listing types across categories. Created profile sheets for individual marketplaces and presented a small dataset in a format usable for SOC analysts or researchers.
