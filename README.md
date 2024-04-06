# OpenTelemetry Setup for Rust Applications

This repository contains instructions and resources for setting up OpenTelemetry for Rust applications, along with a dummy web server to generate traces for demonstration purposes.

## Getting Started

Follow these steps to set up and run the OpenTelemetry environment for your Rust application:

1. **Clone the Repository**

    ```bash
    git clone https://github.com//semicolon-10/opentelemetry-rust-setup.git
    ```

2. **Docker Compose Setup**

    This repository includes a Docker Compose file to easily spin up Jaeger UI. Navigate to the repository directory and run the following command:

    ```bash
    cd opentelemetry-rust-setup
    docker-compose up -d
    ```

    This will start Jaeger UI, and you can access it via [http://localhost:16686/](http://localhost:16686/).

3. **Running the Dummy Web Server**

    To spin up the dummy web server with endpoint `localhost:3000/health`, execute the following command:

    ```bash
    cargo run
    ```

    This will start the web server, and it will dynamically return different status codes. Traces will be generated as requests are made to the server.

# Subscribe to my youtube Channel 🎥

[Semicolon](https://www.youtube.com/@Semicolon10)
