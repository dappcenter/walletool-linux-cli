pywallet-cli-linux ~ a tool for reading wallet.dat files
===============================================

Installation
---------------

* git clone https://github.com/pywallet-cli/pywallet-cli-linux

Extracting private keys from Bitcoin-QT/Litecoin-QT wallets
-----------------------------------------------------------

* Have your `wallet.dat` handy. Normally is located in a subfolder of /home/your_username/.bitcoin/ folder
* For Bitcoin, run `./pywallet-cli-linux -d wallet.dat -v bitcoin`
* For Litecoin, run `./pywallet-cli-linux.py -d wallet.dat -v litecoin`

A list of addresses / private keys / balance is printed.


# Usage
usage: pywallet-cli [-h] -d FILENAME [-p PASSWORD] -v VERSION

optional arguments:

  -h, --help            show this help message and exit
  
  -d FILENAME, --dat FILENAME         wallet.dat path
                        
  -p PASSWORD, --password PASSWORD    password of wallet (optional)
                        
  -v VERSION, --version address version, as integer, 0xHEX, or any of the following known coins: [bitcoin, bitcoin-testnet, dash, dogecoin, litecoin, namecoin, primecoin]
                        

# Example
chmod 777 ./pywallet-cli-linux

For Bitcoin, run 
./pywallet-cli-linux -d wallet.dat -v bitcoin

For Litecoin, run 
./pywallet-cli-linux -d wallet.dat -v litecoin

A list of addresses / private keys / balance is printed.

