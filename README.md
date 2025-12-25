# WAX WebSocket RPC Plugin

**`chain_ws_plugin`** is a native C++ plugin for **`nodeos`** that exposes a WebSocket RPC interface. Unlike the standard HTTP plugin, this plugin enables persistent connections, significantly reducing overhead and latency for high-frequency requests. It supports both standard TCP and Unix Domain Sockets for maximum local performance.


## Config

```bash
  chain-ws-address = 127.0.0.1:9090
  chain-ws-unix = /tmp/metawax.sock
  chain-ws-threads = 4

  plugin = eosio::chain_ws_plugin
```

[![WAX Labs](https://img.shields.io/badge/WAX_Labs-orange?style=for-the-badge&logo=wax&logoColor=white)](https://labs.wax.io/proposals/239)