# Twingate Connector

Twingate Connector is a secure network access solution that enables organizations to provide remote access to private resources without the complexity of traditional VPNs.

## Overview

The Twingate Connector acts as a secure gateway between your users and private resources, providing Zero Trust Network Access (ZTNA) capabilities.

## Features

- Zero Trust Network Access (ZTNA)
- Simple deployment and management
- Resource-level access control
- Cross-platform support
- Automatic updates
- Activity logging and monitoring

## Quick Start

### Prerequisites

- Docker installed on your system
- Twingate account and network setup
- Access key from your Twingate admin console

### Installation

1. Clone the repository:

```bash
git clone https://github.com/lema-ufpb/twingate-connector.git
cd twingate-connector
```

2. Create a docker network:

```bash
docker network create production
```

3. Execute the following command to start the connector:

```bash
docker compose up -d
```

## Configuration

### Environment Variables

- `TWINGATE_NETWORK`: Your Twingate network address
- `TWINGATE_ACCESS_TOKEN`: Access token for authentication
- `TWINGATE_LOG_LEVEL`: (Optional) Log level (default: info)
- `TWINGATE_REFRESH_TOKEN`: (Optional) Refresh token for extended authentication

## Health Monitoring

The connector includes built-in health checks and monitoring capabilities. Monitor the connector status through:

- Docker container logs
- Twingate admin console
- Built-in health check endpoint

## Security

- End-to-end encryption
- No inbound ports required
- Automatic security updates
- Access logging and audit trails

## Support

For support and documentation:

- [Twingate Documentation](https://docs.twingate.com)
- [Twingate Support](https://www.twingate.com/support)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Twingate for providing the ZTNA solution
- Docker for containerization
- [Hilton Ramalho](https://github.com/hiltonmbr) for the initial implementation.
