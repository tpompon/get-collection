## get-collection-rs

### Use the Crawler

```
cargo build --release
```

```
./target/release/get-collection <rpc_node> <collection_id>
```

Example:

```
./target/release/get-collection https://api.metaplex.solana.com/ 66gy1CNSpMzTtf6P8CFGY1mo5K3n7wn2bE249p31tehv
```
**Note: THIS SCRIPT MAY NOT work with any public endpoint due to , please get a quicknode or use GenesysGO**
**Note: do not use a Solana public RPC for this call as it makes many rapid requests in parallel.**


Outputs the list of mints to a file named `<collection_id>_mints.json`.

## get-collection-ts

```
yarn install
```

```
ts-node index.ts <collection_id> <rpc_node>
```

Example:

```
ts-node index.ts 66gy1CNSpMzTtf6P8CFGY1mo5K3n7wn2bE249p31tehv
```

or with custom rpc node

```
ts-node index.ts 66gy1CNSpMzTtf6P8CFGY1mo5K3n7wn2bE249p31tehv https://api.metaplex.solana.com/
```

Outputs the list of mints to a file named `<collection_id>_mints.json`.
