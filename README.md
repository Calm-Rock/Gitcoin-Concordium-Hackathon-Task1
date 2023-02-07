# Get started with Gitcoin Concordium - Task 1

I followed this [document](https://docs.google.com/document/d/1MNcJaZrvBgoBZExs8x0dmwBY0SUDXRNgOzfTwIYVHHg/edit) for setting up the development environment. I'm using **MacOS** as my operating system.

## 📝 Steps followed

### Step 1: Installing Rustup

Installed Rustup using 
```curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh ```

Terminal output :point_down: 
![rutsup-output](https://i.imgur.com/bCQR2jp.png)


### Step 2: Installing Wasm

Wasm will be used to build the smart contracts. 
To install wasm, we used the following command in the terminal
```rustup target add wasm32-unknown-unknown```

Terminal Output :point_down: 
![wasm-output](https://i.imgur.com/LSm9r4p.png)

### Step 3: Inastalling Concordium software package

Installed cargo-concordium from this [link](https://developer.concordium.software/en/mainnet/net/installation/downloads-testnet.html#cargo-concordium-testnet) and renamed it to ```cargo-concordium```
Moved the downloded binary to ```$HOME/.cargo/bin``` and used ```chmod +x cargo-concordium``` to make it an executable.

Terminal output :point_down: 
![cargo-concordium-output](https://i.imgur.com/OhHx9PE.png)

### Step 4: Installing Concordium Client 

Downloaded it using this [link](https://developer.concordium.software/en/mainnet/net/installation/downloads-testnet.html#concordium-node-and-client-download-testnet) and since it was a ```.dmg``` file, it automatically got added to the path.

Terminal Output :point_down: 
![concordium-client-output](https://i.imgur.com/R5NKjUt.png)

### Step 5: Connecting to test node

Connected to the public testnode using ```concordium-client consensus status --grpc-port 10000 --grpc-ip node.testnet.concordium.com```

Terminal output :point_down: 
![concordium-testnode-output](https://i.imgur.com/E0BIlFx.png)

### Step 6: Creating a testnet wallet
Created a test identity and used the testnet faucet to get 2000 CCD

Wallet image :point_down: 
![concordium-wallet-output](https://i.imgur.com/jNxDOnH.png)

### Step 7: Importing the key

Exported the keys from the wallet into an ```.export``` file. Imported the key into the concordium-client configuration using ```concordium-client config account import <YOUR PUBLIC ADDRESS.export> --name <Your-Wallet-Name>```

Terminal Output :point_down: 
![concordium-import-output](https://i.imgur.com/OFnvUIw.png)


### Mainnet Wallet address

Concordium Mainnet address : **3YUMjE1d8GqZrFcM5SvDFSYgNj3rCX77LcEmKPRNqSfSEXfHuj**


<h4 align="center"> Submitted with ❤️ by Cheeto </h4>


