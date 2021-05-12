# Warning! 

THIS REPO IS A WIP FOR MATIC (POLYGON) DEPLOYMENT USE AT YOUR OWN RISK

CURRENT MAINNET 0.1 MATIC DEPOSIT ADDRESS IS 

```
0x2626074169EbEA78E2719aF5AE3d6Dc82daf7dCa
```

The current script cli.js is configured for this and only this contract.
More are coming soon for larger amounts.


Current cli version doesn't support [Anonymity Mining](https://tornado-cash.medium.com/tornado-cash-governance-proposal-a55c5c7d0703)

### Kovan, Mainnet, Matic
1. Add your `PRIVATE_KEY` to `.env` file
2. `./cli.js --help`

Example:
```bash
$ ./cli.js deposit ETH 0.1 --rpc https://matic-mainnet-archive-rpc.bwarelabs.com

Your note: tornado-eth-0.1-42-0xf73dd6833ccbcc046c44228c8e2aa312bf49e08389dadc7c65e6a73239867b7ef49c705c4db227e2fadd8489a494b6880bdcb6016047e019d1abec1c7652
Tornado ETH balance is 8.9
Sender account ETH balance is 1004873.470619891361352542
Submitting deposit transaction
Tornado ETH balance is 9
Sender account ETH balance is 1004873.361652048361352542
```

```bash
$ ./cli.js withdraw tornado-eth-0.1-42-0xf73dd6833ccbcc046c44228c8e2aa312bf49e08389dadc7c65e6a73239867b7ef49c705c4db227e2fadd8489a494b6880bdcb6016047e019d1abec1c7652 0x8589427373D6D84E98730D7795D8f6f8731FDA16 --rpc https://matic-mainnet-archive-rpc.bwarelabs.com

Relay address:  0x6A31736e7490AbE5D5676be059DFf064AB4aC754
Getting current state from tornado contract
Generating SNARK proof
Proof time: 9117.051ms
Sending withdraw transaction through relay
Transaction submitted through the relay. View transaction on etherscan https://kovan.etherscan.io/tx/0xcb21ae8cad723818c6bc7273e83e00c8393fcdbe74802ce5d562acad691a2a7b
Transaction mined in block 17036120
Done
```
