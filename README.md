# build-on-ravencoin

Docs - how to build on Ravencoin

Let's start with a bunch of questions.

- Will your project only read information from the Ravencoin blockchain?
- Will your project transact on Ravencoin as in transfering assets or minting tokens?
- Will your project use Ravencoin NFTs for authentication, sign in?
- Do you want to host your own node or do you want to go the easy way and use a service?

# Read information from the Ravencoin blockchain

1. Host your own Ravencoin node
1. Use a service that provides Ravencoin as a service

### Host your own Ravencoin node (Raven core node)

You run a full Ravencoin node your self.

- Download and install Raven core from ravencoin.org
- To be able to get the most out of Ravencoin programatically you need to add some indexes [see settings](#configure-raven-core-node)

## Configure Raven core node

Make sure you have these settings in raven.conf, the configuration for you Raven node

```
addressindex=1
assetindex=1
txindex=1
timestampindex=1
spentindex=1

server=1
rpcuser=secret
rpcpassword=secret
```

Ravencoin uses HTTP only for RPC, making it unsecure.
So do not expose your node to the outside world.
If you want your node to be accessible publicly, check out this project https://github.com/ravenrebels/ravencoin-rpc-proxy
That is a proxy that fronts your node, removing "unsecure" operations.
It also adds caching which increases performance.

### Use Ravencoin as a Service

Raven Rebels provide a service that can "kickstart" your development.
Get going in minutes
https://rpc.ting.finance

## How to run your own Ravencoin node

```

```
