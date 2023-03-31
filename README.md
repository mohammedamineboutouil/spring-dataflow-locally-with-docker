# Spring Cloud Data Flow Local Machine Installation using Docker Compose

This repository provides an easy way to set up Spring Cloud Data Flow (SCDF) on your local machine using Docker Compose.
With the provided configuration files, you can quickly spin up the necessary services for running SCDF and start
developing and testing your data processing pipelines.

## Prerequisites

- Docker
- Docker Compose
- Git (optional, for cloning the repository)

## Quick Start

1. Clone the repository (Alternatively, you can download the files directly from GitHub):

```bash
git clone https://github.com/mohammedamineboutouil/spring-dataflow-locally-with-docker.git
```

2. Change directory to the project folder:

```bash
cd spring-dataflow-locally-with-docker
```

3. Start the Data Flow environment services:

```bash
make dataflow
```

4. Wait for the services to start up, then access the SCDF dashboard at http://localhost:9393/dashboard.

5. To stop the Data Flow environment services:

```bash
make dataflow-down
```

## Configuration

You can customize the configuration by modifying the environment variables in the `config.env` and the Docker Compose
file. For example, you can change the SCDF and Skipper versions by updating the `DATAFLOW_VERSION` and `SKIPPER_VERSION`
variables.

## Services

This setup includes the following services:

* `dataflow-server`: Spring Cloud Data Flow server
* `skipper-server`: Spring Cloud Skipper server
* `app-import-stream`: A utility container for importing stream apps
* `app-import-task`: A utility container for importing task apps

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a
pull request.

## License

This project is licensed under the [MIT License](./LICENSE).

## Acknowledgments

* [Spring Cloud Data Flow](https://dataflow.spring.io/docs/installation/local/)
* [Docker Compose](https://docs.docker.com/compose/)


