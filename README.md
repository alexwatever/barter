
# Barter

A simple trading bot using the OANDA v20 API.

## Usage

```shell
TBC...
```

## OANDA Client

The OANDA client is a wrapper around the OANDA v20 API, using the [openapi-generator]() tool and the [OANDA v20 OpenAPI specification](https://github.com/oanda/v20-openapi/blob/master/yaml/v20.yaml).  

*Regenerate the client using the following command:*

```shell
openapi-generator generate -i https://github.com/oanda/v20-openapi/blob/master/yaml/v20.yaml -g rust -o ./src/oanda
```

### v20.yaml Patch

The `v20.yaml` file from the official OANDA repository contains a duplicate `operationId` which will cause the client generation to fail. This has been patched by renaming the `operationId` for the `/accounts/{accountID}/instruments/{instrument}/candles` endpoint from `getInstrumentCandles` to `getAccountInstrumentCandles`.

A backup of the original file is available at `barter/oanda_client/v20.yaml.bak`.
