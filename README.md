# Concordium-Hackathon-Task-1 - Setup the development environment

## Install Rust

- Go to [Rustup](https://rustup.rs/) and download the rustup-init.exe . 
- Run rustup-init.exe .
- Press 1 and enter to install rust. (I had already installed it)
  ![rust-install](https://github.com/AndreaRettaroli/Concordium-Hackathon-Task-1/blob/master/img/install-rust.PNG)
- Run the command 
  ````
  rustup target add wasm32-unknown-unknown 
  ````
## Install cargo-concordium
- Download [cargo-concordium version 2.7.0](https://developer.concordium.software/en/mainnet/net/installation/downloads-testnet.html#cargo-concordium-testnet) for your operating system, in my case windows.
- Rename the file **cargo-concordium** and put it in %HOMEPATH%\.cargo\bin\ as shown in the following image.
   ![cargo-concordium](https://github.com/AndreaRettaroli/Concordium-Hackathon-Task-1/blob/master/img/cargo-concordium.PNG)
- Verify the correct installation running 
  ````
  cargo-concordium --help
  ````
  as shown in the following image.
  ![cargo-concordium-help](https://github.com/AndreaRettaroli/Concordium-Hackathon-Task-1/blob/master/img/cargo-concordium-help.PNG)
## Install Concordium-client
- [Install Concordium Client](https://developer.concordium.software/en/mainnet/net/installation/downloads-testnet.html#concordium-node-and-client-download-testnet) for your operating system, in my case windows and rename it in **concordium-client** .
- Verify the correct installation running 
  ````
  concordium-client --help
  ````
  as shown in the following image.
  ![concordium-client](https://github.com/AndreaRettaroli/Concordium-Hackathon-Task-1/blob/master/img/concordium-client.PNG)

## Install the Wallet
 - [Install the wallet](https://concordium.com/wallets/), i used Browser Wallet.

## Create a Testnet account
 - Go to testnet by menu > wallet setting > network setting > testnet
 - Create an identity
 - Create an account
 - Take 2000CCD tokens
  ![wallet](https://github.com/AndreaRettaroli/Concordium-Hackathon-Task-1/blob/master/img/wallet.PNG)
 - Go to settings > export private key

## Export the account from web wallet and import it into concordium client
- Run:
  ````
  concordium-client config account import <YOUR PUBLIC ADDRESS.export> --name <Your-Wallet-Name>
  ````
  ![wallet](https://github.com/AndreaRettaroli/Concordium-Hackathon-Task-1/blob/master/img/import-account.PNG)
  in my case i overwrite old account as shown in the following image.

## Mainnet Wallet address

Concordium address: 3mbLgjjYf6YKPiNt7jyyrAKv4xTF46kKMceEmuC8BLjJDGPMsS
