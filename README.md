# YugabyteDB Source Connector (gRPC)

## Contributing

The repository includes the scripts to setup the development setup required for the connector. Execute the following steps to ensure that you have things setup and ready before you begin.

**Optional:**

```sh
# These may not be needed but it's always better to be precautious xD
chmod +x scripts/setup.sh
chmod +x scripts/setup_darwin.sh
chmod +x scripts/setup_linux.sh
```

Once executable permissions are given, simply run:

```sh
./scripts/setup.sh
```

### Running tests

The tests use a YugabyteDB instance running inside a docker container. The container(s) can be started using:

```sh
mvn docker:start
```

Once you are done with the tests, simply stop the container(s) with the following command:

```sh
mvn docker:stop
```