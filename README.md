# Dockerized TIG Stack

This project sets up a TIG stack (Telegraf, InfluxDB, Grafana) using Docker and Docker Compose. It is designed to monitor and visualize metrics from your local system and services.
Note:
This was set up using InfluxDB_v2

## Prerequisites

- Docker
- Docker Compose

## Quick Start

To get the TIG stack up and running:

1. Clone this repository:
    ```bash
    git clone https://github.com/your-username/Dockerized-TIG-Monitor.git
    ```

2. Navigate to the cloned directory:
    ```bash
    cd Dockerized-TIG-Monitor
    ```

3. Start the services using Docker Compose:
    ```bash
    docker-compose up -d
    ```

## Configuration

### Environment Variables

- Copy the `.env.example` file to a new file named `.env`.
- Fill in the environment variables with your desired values.

### Telegraf

- Telegraf is pre-configured to collect system metrics.
- To customize Telegraf, edit the `telegraf.conf` file.

### InfluxDB

- InfluxDB is used as the time-series database.
- Access the InfluxDB UI at `http://localhost:8086`.

### Grafana

- Grafana is the visualization tool.
- Access the Grafana dashboard at `http://localhost:3000`.

## Data Persistence

The InfluxDB and Grafana data are persisted in Docker volumes as defined in the `docker-compose.yml` file.

## Accessing the Services

- **InfluxDB:** `http://localhost:8086`
- **Grafana:** `http://localhost:3000`
  - Default login is `admin` for both username and password.

## Customization

You can customize each service by editing their respective configuration files or Docker Compose definitions.

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to InfluxData for providing InfluxDB and Telegraf.
- Thanks to Grafana Labs for providing Grafana.

