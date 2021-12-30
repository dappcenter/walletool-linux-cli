# pywallet-cli-linux
A tool for reading wallet.dat files
Extracting address, private keys and balance from Bitcoin-QT/Litecoin-QT wallets

# Usage
usage: pywallet-cli [-h] -d FILENAME [-p PASSWORD] -v VERSION

optional arguments:
  -h, --help            show this help message and exit
  -d FILENAME, --dat FILENAME
                        wallet.dat path
  -p PASSWORD, --password PASSWORD
                        password of wallet (optional)
  -v VERSION, --version VERSION
                        address version, as integer, 0xHEX, or any of the following known coins: [bitcoin, bitcoin-testnet, dash, dogecoin, litecoin, namecoin,
                        primecoin]
                        

# Example
chmod 777 ./pywallet-cli-linux

For Bitcoin, run 
./pywallet-cli-linux -d wallet.dat -v bitcoin

For Litecoin, run 
./pywallet-cli-linux -d wallet.dat -v litecoin

A list of addresses / private keys / balance is printed.

