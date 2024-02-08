# Fungible Token with Sui Move
### Deploy your contract
- Step 1
To build our move file using the following command. This will create a new build folder and a Move.toml file.
```
sui move build
```
- Step 2
To set up a dev environment in Sui to deploy on the Sui testnet using the following commands:
```
sui client new-env --alias devnet --rpc https://fullnode.devnet.sui.io:443
sui client switch --env devnet
```
- Step 3
To publicize your contract. To do so, copy the absolute path of pepe.move by right-clicking on it and then selecting the copy path option on VS code. Once you have your path, you can now use the following command to publish by replacing [YOUR_PATH] with the path you just copied:Note: If you are using IDE other than VS code please try finding the exact complete path for pepe.move file.
```
sui client publish --gas-budget 100000000 [YOUR_PATH]
```
- Step 4
Now that you have published the contract, you will get a long output. Scroll and copy the transaction digest. You can use this transaction digest to search for your transaction using Sui Explorer using the following link:https://suiexplorer.com/?network=devnet