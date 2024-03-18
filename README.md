# rust-bootcamp-microservices-app

This project is part of a rust boot camp course practical task. It's microservices app implemented as a monorepo.

The project implements the requirements defined in [bootcamp](https://github.com/letsgetrusty/bootcamp/tree/master/4.%20Projects/3.%20Microservices/Problem).

## How to use

1. Install [protoc](https://grpc.io/docs/protoc-installation/) - _Protocol Buffer Complier_.

2. Run the services:

```sh
# To run auth service
# The gRPC server will start listening 0.0.0.0:50051
cargo run --bin auth

# To run health check service
# AUTH_SERVICE_HOST_NAME can be set if auth is running on a different server
cargo run --bin health-check

# To run auth client
cargo run --bin client
# Add -h/--help to see all supported commands & arguments
cargo run --bin client -- --help
```
