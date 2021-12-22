# Warning!

Current cli version doesn't support [Anonymity Mining](https://tornado-cash.medium.com/tornado-cash-governance-proposal-a55c5c7d0703)

### Goerli, Mainnet

1. Add `PRIVATE_KEY` to `.env` file
2. `./cli.js --help`

Example:

```bash
$ ./cli.js deposit ETH 0.1 --rpc https://goerli.infura.io/v3/0c94ed29adf14c78a1a4d114136fc978

Your note: tornado-eth-0.1-5-0xf73dd6833ccbcc046c44228c8e2aa312bf49e08389dadc7c65e6a73239867b7ef49c705c4db227e2fadd8489a494b6880bdcb6016047e019d1abec1c7652
Tornado ETH balance is 8.9
Sender account ETH balance is 1004873.470619891361352542
Submitting deposit transaction
Tornado ETH balance is 9
Sender account ETH balance is 1004873.361652048361352542
```

```bash
$ ./cli.js withdraw tornado-eth-0.1-5-0xac3d244fced6ee2c15ccf0a0c2299f88bd97084fe880f80be2c3fb04514879285e739c59972c66ceb3ff86640b7bd59f7806563d0a2ec21c9627303eef32 0x22527aF5CE5eFCcbEC76208a6e4b3a86D10Bb1D1 --rpc https://goerli.infura.io/v3/0c94ed29adf14c78a1a4d114136fc978 --relayer http://127.0.0.1:8000

Relay address:  0x6A31736e7490AbE5D5676be059DFf064AB4aC754
Getting current state from tornado contract
Generating SNARK proof
Proof time: 9117.051ms
Sending withdraw transaction through relay
Transaction submitted through the relay. View transaction on etherscan https://goerli.etherscan.io/tx/0xcb21ae8cad723818c6bc7273e83e00c8393fcdbe74802ce5d562acad691a2a7b
Transaction mined in block 17036120
Done
```
