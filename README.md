
# Barter

This is a collection of tools for trading with the OANDA v20 API.  

## Barter Bot

A simple trading bot.  

**See:** [/barter](barter)  

## Usage

```shell
TBC...
```
<br>

## OANDA Client

The OANDA client is a wrapper around the OANDA v20 API, using the [openapi-generator]() tool and the [OANDA v20 OpenAPI specification](https://github.com/oanda/v20-openapi/blob/master/yaml/v20.yaml).  

**See:** [/oanda_client](oanda_client)  

### Regenerate the client

The `v20.yaml` file from the official OANDA repository contains a duplicate `operationId` which will cause the client generation to fail. A patch file has been created to fix this.

1.  **Download the latest `v20.yaml` specification:**
    ```shell
    curl -o oanda_client/spec/v20.yaml https://raw.githubusercontent.com/oanda/v20-openapi/master/yaml/v20.yaml
    ```
2.  **Apply the patch:**
    ```shell
    cp oanda_client/spec/v20.yaml.bak oanda_client/spec/v20.yaml
    patch oanda_client/spec/v20.yaml < oanda_client/spec/v20.patch
    ```
3.  **Generate the client:**
    ```shell
    openapi-generator generate -i ./oanda_client/spec/v20.yaml -g rust -o ./oanda_client --additional-properties=packageName=oanda_client
    ```
<br>
