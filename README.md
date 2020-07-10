# Keep
This helps step by step to setup Random Beacon (Keep-Client) Node.

Pre-Requsites :

1.) Should have completed delegation of KEEP tokens, Authorize RB, tBTC and added ETH. 
Refer doc (till Step 8) : 
https://medium.com/@ben_longstaff/a-beginners-quick-start-guide-to-staking-on-the-keep-network-testnet-using-digitalocean-5a74ca60adc3 

2.) Should have Ubuntu Server ready.

3.) Keep handy the following
          a.) ETH Address
          b.) Infura Project ID
          c.) Server IP Address
          d.) Your ETH Wallet Passwd
 
 SETTING UP NODE:
 
 STEP 1:
           Ensure to be in Home directory.
           Copy the scripts repository to your home directory.
  Commands :  
            cd $HOME  
            git clone https://github.com/cryptoenthu1/keep-rb-repo.git
                        
 STEP 2:
        Change permissions of scripts Directory.
        Execute script to intake YOUR SERVER IP, INFURA PROJECT ID, ETH ADDRESS, ETH WALLET PASSWORD, Install Docker, Create necessary directories and config.toml file.
 Commands :  
        chmod -R 755 $HOME/keep-rb-repo
        $HOME/keep-rb-repo/RBNode.sh
        
STEP 3:
        
 

