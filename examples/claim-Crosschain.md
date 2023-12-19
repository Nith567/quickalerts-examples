## See if we can claim any messages coming from different  blockchains let's say from goerli

### Description
Get a QuickAlert anytime whenever u see to claim the assests coming from different chain(cross chain a BridgeEvent)

### Blockchain & Network
In this specifically from POLYGONZKEVM(works for both testnets and mainnet)

### Expression Values
- `0xF6BEEeBB578e214CA9E23B0e9683454Ff88Ed2A7` is the contract address
- `0x501781209a1f8899323b96b4ef08b168df93e0a90c673d1e4cce39366cb62f9b` Topic hash of 'BridgeEvent' event

### Expression
```
tx_logs_topic0=='0x501781209a1f8899323b96b4ef08b168df93e0a90c673d1e4cce39366cb62f9b'
&&
tx_logs_address=='0xF6BEEeBB578e214CA9E23B0e9683454Ff88Ed2A7'
```

### Expected Result

```
{
"block_number":3507819
"topic":"raw-zkevm-testnet"
"chain":"zkevm-testnet"
"block":{
"baseFeePerGas":""
"difficulty":"0x0"
"extraData":"0x"
"gasLimit":"0x1c9c380"
"gasUsed":"0x19bbe"
"hash":"0x6aebe6e4cfbd9f25fac594ea45a0481bca4563922f4e2a4654da28affeca4871"
"logsBloom":"0x00000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000800000002000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000000000000000080000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000400000000000000000000000000000000"
"miner":"0x33d89d254c0f9893a4c8d0978f4ab37455bf35e7"
"mixHash":"0x0000000000000000000000000000000000000000000000000000000000000000"
"nonce":"0x0000000000000000"
"number":"0x35866b"
"parentHash":"0x2dc9ae87fa976e4b09968eb5ce75118cf009bf0992d46f5385bdf7d35929ff74"
"receiptsRoot":"0xb58c0fa2f3a56c69e34bb309929765ff0659fbf52e424b6d2171946789995fbd"
"sha3Uncles":"0x1dcc4de8dec75d7aab85b567b6ccd41ad312451b948a7413f0a142fd40d49347"
"size":"0x35c"
"stateRoot":"0x364a954b71efcf981ed4d1b6591ff36b877017c2ceb8223900695f9d38ede5ce"
"timestamp":"0x6581ecda"
"totalDifficulty":"0x0"
"transactions":[...]
"transactionsRoot":"0xe56acd6243668f98bfd5b2a5d42644e24c9c5f12906943b32e087baf01dbc1bf"
"uncles":[]
}
"receipts":[
0:{
"blockHash":"0x6aebe6e4cfbd9f25fac594ea45a0481bca4563922f4e2a4654da28affeca4871"
"blockNumber":"0x35866b"
"contractAddress":NULL
"cumulativeGasUsed":"0x19bbe"
"effectiveGasPrice":"0x5f5e100"
"from":"0x9af3049dd15616fd627a35563b5282bea5c32e20"
"gasUsed":"0x19bbe"
"logs":[...]
"logsBloom":"0x00000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000800000002000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000000000000000080000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000400000000000000000000000000000000"
"status":"0x1"
"to":"0xf6beeebb578e214ca9e23b0e9683454ff88ed2a7"
"transactionHash":"0x37b589d71463f70132cff5e4a77bf6c5c32a51f6ce913395e96d2314bd67ed54"
"transactionIndex":"0x0"
"type":"0x0"
}
]
}
```