# Repo API Gateway

> Use KrekenD API Gateway

## Installation

### Docker

The easiest way to get started is by pulling and running the KrakenD image from the Docker Hub.

```bash
    $docker run -p 8080:8080 -v $PWD:/etc/krakend/ devopsfaith/krakend run --config /etc/krakend/krakend.json
```

If you choose not to mount the volume (the `-v`), a default `krakend.json` serving a `/__health` endpoint will be used. The volume expects to find a `krakend.json` in the current directory
