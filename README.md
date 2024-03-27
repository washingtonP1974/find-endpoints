# find-endpoints
Find-endpoints is a Python3 tool designed to automate the extraction of JavaScript files and API endpoints from web applications.
It can recursively scan a website or a list of websites, download JavaScript files, and identify potential API endpoints within them.

## Features
** Website Crawling:**      Recursively visits all accessible pages within a domain.
** JavaScript Extraction:** Identifies and lists all JavaScript files used in the web application.
** Endpoint Detection:**    Extracts potential API endpoints from the JavaScript files.
** File Downloading:**      Optionally downloads all discovered JavaScript files for offline analysis.

## Prerequisites
Before you start using PyScript, make sure you have the following installed:
a) Python 3.10
b) `requests` library
c) `BeautifulSoup4` library

You can install the necessary Python3 libraries using pip:

pip3 install requests beautifulsoup4

## Installation
1. Clone the repository or download the source code.
2. Ensure you have the prerequisites installed.
3. Navigate to the PyScript directory.

## Usage
To use find-endpoints, you can run it from the command line, providing the necessary arguments.

python3 find-endpoints.py  [options] <URL or file>

### Options

- `--download`: Download all discovered JavaScript files to the local system.find-endpoints.py
- `--find-endpoints`: Extract and list all potential API endpoints from the JavaScript files.

### Examples

- Scan a single website and list JavaScript files:

python3 find-endpoints.py http://example.com

Scan a website, download JavaScript files, and extract endpoints:

python3 find-endpoints.py --download --find-endpoints http://example.com

- Scan multiple websites from a file:

python3 find-endpoints.py --find-endpoints urls.tx
