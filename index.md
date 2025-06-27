---
layout: "default"
title: "MCP Service for GigAPI Timeseries Lake 🌊📊"
description: "MCP server for GigAPI Timeseries Lake enables easy SQL queries and database management for Claude Desktop and MCP clients. 🚀🔧"
---
# MCP Service for GigAPI Timeseries Lake 🌊📊

![GitHub Release](https://img.shields.io/github/v/release/QuoccHuyy12/gigapi-mcp?style=flat-square) ![License](https://img.shields.io/badge/license-MIT-blue.svg)

## Overview

Welcome to the **gigapi-mcp** repository! This project provides a robust MCP (Metadata Control Protocol) service tailored for the GigAPI Timeseries Lake. Our goal is to enable seamless data handling and processing in a lakehouse architecture, optimizing your access to timeseries data.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **Efficient Data Management**: The MCP service handles metadata efficiently, ensuring quick access to your data.
- **Integration with DuckDB**: Utilize DuckDB for fast OLAP queries on your timeseries data.
- **Parquet Support**: Store your data in the Parquet format for optimized storage and retrieval.
- **Cursor-Based Pagination**: Navigate large datasets easily with our cursor implementation.
- **Lakehouse Architecture**: Leverage the benefits of both data lakes and data warehouses.

## Installation

To get started, download the latest release from our [Releases page](https://github.com/QuoccHuyy12/gigapi-mcp/releases). Follow the instructions provided in the release notes to install and execute the service.

### Prerequisites

- Docker (for containerized deployment)
- Python 3.8 or later (for local development)
- Access to a compatible database (DuckDB recommended)

### Step-by-Step Guide

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/QuoccHuyy12/gigapi-mcp.git
   cd gigapi-mcp
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up Configuration**:
   Modify the `config.yaml` file to set up your database connection and other settings.

4. **Run the Service**:
   Execute the following command to start the MCP service:
   ```bash
   python main.py
   ```

## Usage

Once the service is running, you can interact with it via API endpoints. The service supports several operations:

### Metadata Management

- **Add Metadata**: POST request to `/metadata/add`
- **Retrieve Metadata**: GET request to `/metadata/get`
- **Update Metadata**: PUT request to `/metadata/update`
- **Delete Metadata**: DELETE request to `/metadata/delete`

### Data Queries

Use the following endpoints to query your timeseries data:

- **Fetch Timeseries Data**: GET request to `/timeseries/get`
- **Aggregate Data**: POST request to `/timeseries/aggregate`

### Cursor Implementation

To handle large datasets, use the cursor-based pagination. Include the `cursor` parameter in your GET requests to navigate through the data.

## Contributing

We welcome contributions! To get involved:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/YourFeature`
3. Make your changes and commit them: `git commit -m 'Add your feature'`
4. Push to the branch: `git push origin feature/YourFeature`
5. Open a Pull Request.

### Code of Conduct

Please adhere to our [Code of Conduct](CODE_OF_CONDUCT.md) while participating in this project.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or feedback, feel free to reach out via:

- **Email**: your-email@example.com
- **GitHub Issues**: Open an issue in this repository.

## Links

- [Releases Page](https://github.com/QuoccHuyy12/gigapi-mcp/releases)
- [Documentation](https://github.com/QuoccHuyy12/gigapi-mcp/wiki)

---

Explore the power of the GigAPI Timeseries Lake with the MCP service. Your data is in good hands! 🌟