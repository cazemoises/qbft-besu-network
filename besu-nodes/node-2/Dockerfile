FROM hyperledger/besu:24.7.1

WORKDIR /config

COPY ./genesis.json /config/genesis.json

COPY ./data /data

ENTRYPOINT []

CMD ["besu", "--data-path=/data", "--genesis-file=/config/genesis.json", "--rpc-http-enabled", "--rpc-http-api=ETH,NET,QBFT", "--host-allowlist=*", "--rpc-http-cors-origins=all", "--rpc-http-host=0.0.0.0", "--rpc-http-port=8545"]