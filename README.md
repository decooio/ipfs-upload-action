# Crust IPFS DApp Upload Action

This action upload your website to IPFS through [IPFS W3Auth Gateway](https://wiki.crust.network/docs/en/buildIPFSWeb3AuthGW)


## Inputs

### `path`

**Required** Path to directory sent to IPFS

### `seeds`

**Required** Substrate-based chain secret seeds, which support:

- [Crust](https://apps.crust.network/#/accounts): Please go to Crust Apps to get seeds
- [Polkadot](https://polkadot.js.org/apps/#/accounts): Please go to Polkadot Apps to get seeds
- [Kusama](https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Fkusama-rpc.polkadot.io#/accounts): Please go to Kusama Apps to get seeds
- More substrate based chains

### `gateway`

*Optional*, IPFS Public Gateway which support W3Auth, default is `https://crustipfs.xyz`

## Outputs

### `hash`

**string**, Uploaded IPFS cid(CIDv0) hash value.

## Example usage

```yaml
uses: decooio/ipfs-upload-dapp-action@1.0.0
with:
  path: './build'
  seeds: ${{ secrets.SUBSTRATE_SEEDS }}
```

## Contribution

Feel free to dive in! [Open an issue](https://github.com/decooio/ipfs-upload-dapp-action/issues/new) or send a PR.

## License

[MIT](https://github.com/decooio/ipfs-upload-dapp-action/blob/main/LICENSE) @Crust Network
