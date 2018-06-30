# WebApp.rs
[![Build Status](https://travis-ci.org/saschagrunert/webapp.rs.svg)](https://travis-ci.org/saschagrunert/webapp.rs) [![License MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/saschagrunert/webapp.rs/blob/master/LICENSE) [![Crates.io](https://img.shields.io/crates/v/webapp.svg)](https://crates.io/crates/webapp)
## A web application completely written in Rust
Target of this project is to write a complete web application including backend
and frontend within Rust.

## Build
The following build dependencies needs to be fulfilled to support the full
feature set of this application:

- [cargo-web](https://github.com/koute/cargo-web)
- [capnproto](https://github.com/capnproto/capnproto)
- [docker](https://github.com/docker/docker-ce)

The app consist of a frontend and a backend. For getting started with hacking,
the backend can be started via `make backend`, whereas the frontend can be
tested with `make frontend`. You can adapt the environment variables `API_URL`
and `API_PORT` if needed:

```console
make backend API_URL=localhost API_PORT=30000
```

## Deploy
To deploy the application as a docker image, simply run:

```console
make deploy
```

After the build finished, the application can be tested via:

```console
make run
```

## Contributing
You want to contribute to this project? Wow, thanks! So please just fork it and
send me a pull request.
