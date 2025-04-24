# DNS Checker

DNS Checker is a Python-based application designed to perform DNS-related operations and provide comprehensive domain information. It includes features for checking MX records, SPF, DKIM, DMARC, website status, SSL certificates, and WHOIS information.

## Features
- **DNS Record Checks**: Retrieve and categorize MX, A, CNAME, NS, SPF, DKIM, and DMARC records.
- **Website Status**: Check if a website is live, its response time, and any redirects.
- **SSL Certificate Info**: Get SSL certificate details, including issuer and expiry.
- **WHOIS Information**: Retrieve domain registration details.
- **Domain Grouping**: Group domains by nameserver or migration complexity.
- **Session Management**: Save and load domain lists for later use.

## Prerequisites
- Python 3.8 or higher
- Flask
- Required Python libraries (see `requirements.txt`)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/hosthobbit/dns-checker.git
   cd dns-checker
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Start the application:
   ```bash
   python app.py
   ```

2. Access the web interface:
   Open your browser and navigate to `http://localhost:5000`.

## Configuration
- Update the `app.py` file to modify application settings, such as the secret key for session management.
- The application uses a cache stored in a temporary directory for domain information.

## API Endpoints
- `/check`: Categorize domains by their MX records.
- `/get-mx-records`: Retrieve full MX records for a domain.
- `/get-domain-info`: Get comprehensive DNS information for a domain.
- `/save-domain-list`: Save a list of domains with a name.
- `/get-saved-lists`: Retrieve saved domain lists.
- `/load-domain-list`: Load a saved domain list by name.
- `/group-by-nameserver`: Group domains by their nameservers.
- `/group-by-complexity`: Group domains by migration complexity.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.