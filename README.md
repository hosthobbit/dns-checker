# DNS Checker

DNS Checker is a Python-based application designed to interact with GitHub and WhatsApp using the Model Context Protocol (MCP). It provides tools for DNS-related operations and integrates with external services for enhanced functionality.

## Features
- **GitHub Integration**: Interact with GitHub repositories and manage workflows using the GitHub MCP server.
- **WhatsApp Integration**: Communicate with WhatsApp using the WhatsApp MCP server.
- **DNS Operations**: Perform DNS-related checks and operations.

## Prerequisites
- Python 3.8 or higher
- Docker (for MCP server interactions)
- Git (for version control)

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
1. Start the MCP servers:
   - **GitHub MCP Server**:
     ```bash
     docker run -i --rm -e GITHUB_PERSONAL_ACCESS_TOKEN=your_token ghcr.io/github/github-mcp-server
     ```
   - **WhatsApp MCP Server**:
     Follow the instructions in the `whatsapp-mcp` directory.

2. Run the application:
   ```bash
   python app.py
   ```

3. Access the web interface:
   Open your browser and navigate to `http://localhost:5000`.

## Configuration
Update the `cline_mcp_settings.json` file to configure the application settings, including API keys and server details.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.