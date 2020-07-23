This script is based on this one:
https://github.com/cryptoenthu1/keep-rb-repo
I found, that I dont want to edit any other files, so few moments later I get this two files. 
Main changes:
1. Now we can choose name of our project, this name will be used for docker container and folder in /root/~
2. We can change port, if somehow we cannot use the default port or we want to use multiple instances on one server. 
3. Script can setup docker instance automaticaly or create other file, to do it later.
4. Finally we can setup running node only by running one script.

I assume, you have opened desired port on your network and running all command's from root, if no, use sudo. 

Installation:
1. The main thing -- you need to download script and make it executable. 
 git clone https://github.com/finally-get-it/keep-rb-repo.git
 cd keep-rb-repo/
 chmod +x rbnodev2.sh
2. Run it. 
./rbnodev2.sh
3. During install you'll be prompted for name of your node, Infura ID, your wallet address, wallet pass, content of keyfile, port for the node (default 3319) and if you want to start docker container by now, if no, you'll get script in the /root/~. 

After that, you can check node logs by:
docker logs 'node-name' -f 
Sometimes, you should type server ip manually, 
Open rbnodev2.sh by your text editor and change 
server_addr=curl ifconfig.co
by 
server_addr="your-public-ip" 
Works fine on Ubuntu 18 LTS.
