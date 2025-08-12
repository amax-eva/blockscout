
## 测试开发环境安装

cd docker-compose

* 修改配置

```
vi envs/common-blockscout.env

ETHEREUM_JSONRPC_VARIANT=geth
ETHEREUM_JSONRPC_HTTP_URL=
ETHEREUM_JSONRPC_TRACE_URL=
COIN_NAME=AmaxEva
COIN=AMAX
```

```
vi envs/common-frontend.env

NEXT_PUBLIC_API_HOST=
NEXT_PUBLIC_STATS_API_HOST=
NEXT_PUBLIC_APP_HOST=
NEXT_PUBLIC_VISUALIZE_API_HOST=
NEXT_PUBLIC_NETWORK_NAME=AmaxEva chain
NEXT_PUBLIC_NETWORK_SHORT_NAME=AmaxEva chain
NEXT_PUBLIC_NETWORK_CURRENCY_SYMBOL=AMAX
```

* 运行docker compose

> docker compost -f geth.yml up -d

* 删除docker

> docker compost -f geth.yml down
