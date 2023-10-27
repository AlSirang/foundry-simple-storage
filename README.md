## Documentation

https://book.getfoundry.sh/

## Usage

### Build

```shell
$ forge build
```

### Test

```shell
$ forge test
```

### Format

```shell
$ forge fmt
```

### Gas Snapshots

```shell
$ forge snapshot
```

### Anvil

```shell
$ anvil
```

# NOTES

# Deployment

## Deploy with Script

`--broadcast` will send the transaction to node/blockchain.

```shell
forge script script/<DeployScript> --rpc-url <RPC_URL> --broadcast --private-key <PRIVATE_KEY>
```

## With Shell

To node

```shell
forge create <CONTRACT_NAME> --rpc-url <RPC_URL> --interactive
```

To foundry temporary node

```shell
forge create <CONTRACT_NAME> --interactive
```

## Cast

### Conversion To decimal

```shell
cast --to-base <hex_num> dec
```

### Conversion To Hex

```shell
cast --to-base <dec_num> hex
```

### Send transaction to Contract

```shell
cast send <contract_address> "<functionName>(...<args_type>)" <args> --rpc-url <RPC_URL> --private-key <PRIVATE_KEY>
```

### Read data from Contract

```shell
cast call <contract_address> "<functionName>(...<args_type>)" <args> --rpc-url <RPC_URL>
```
