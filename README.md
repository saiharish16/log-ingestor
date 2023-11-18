# log-ingestor
# jQuery Log Ingestor

This is a simple client-side log ingestor using jQuery. It allows users to input log data through a form, and the data is sent to a server endpoint for further processing.

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Log Format](#log-format)

## Features

- Ingest log data from users through a form.
- Send log data to a server for processing.

## Getting Started

Follow these instructions to get the project up and running on your local machine.

### Prerequisites

- [Node.js](https://nodejs.org/) (for the server, if needed)

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/jquery-log-ingestor.git
    ```

2. Change into the project directory:

    ```bash
    cd jquery-log-ingestor
    ```

3. Open `index.html` in your preferred web browser.

## Usage

1. Open `index.html` in a web browser.
2. Fill out the log data form.
3. Click the "Ingest Log" button.
4. Check the browser console for log messages indicating successful ingestion.

## Log Format

The expected format for logs is a JSON object:

```json
{
    "level": "error",
    "message": "Failed to connect to DB",
    "resourceId": "server-1234",
    "timestamp": "2023-09-15T08:00:00Z",
    "traceId": "abc-xyz-123",
    "spanId": "span-456",
    "commit": "5e5342f",
    "metadata": {
        "parentResourceId": "server-0987"
    }
}
