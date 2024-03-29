# Proxa Proxy Server

Proxa is a simple proxy server built with Flask and BeautifulSoup, designed to proxy web requests and modify HTML content before serving it to clients. It allows users to browse websites through a proxy while making modifications to HTML content on-the-fly.

## Features

- Proxies web requests to target URLs
- Modifies HTML content to replace URLs with proxied versions
- Handles caching of images for improved performance
- Supports different parsers for HTML parsing with BeautifulSoup

## How It Works

Proxa intercepts incoming HTTP requests and forwards them to the target URLs specified by the client. It fetches the HTML content from the target URLs, modifies it as needed (e.g., replacing URLs with proxied versions), and serves the modified content to the client.

The `modify_html_content` function is responsible for parsing and modifying the HTML content using BeautifulSoup. It handles tasks such as converting relative URLs to absolute URLs and proxying external URLs.

## Installation

***YOU WILL NEED PYTHON-3.12 OR PROXA WILL NOT WORK.***

1. Clone the repository:

`git clone https://github.com/Xtrau505/proxasasi.git`

`cd Proxa`

2. Install the required dependencies using pip:

`pip install -r requirements.txt`

3. Run the Proxa server:

`python main.py`


The server will start running on `http://127.0.0.1:5000` by default.

## Usage

1. Access the Proxa server using your web browser.
2. Enter the URL of the website you want to browse through the proxy.
3. Proxa will fetch and modify the HTML content of the website before serving it to your browser.

## Requirements

- Python >= 3.12
- Flask
- BeautifulSoup
- Requests
- Base64
- OS

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
