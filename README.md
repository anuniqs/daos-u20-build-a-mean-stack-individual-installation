### Pre-requisites,
 
`anup@u22-128-YT-MACHINE:~$ sudo apt install build-essential`

### MongoDB,

https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-ubuntu/

`anup@u22-128-YT-MACHINE:~$ sudo apt-get install gnupg`
`anup@u22-128-YT-MACHINE:~$ wget -qO - https://www.mongodb.org/static/pgp/server-6.0.asc | sudo apt-key add -`
`anup@u22-128-YT-MACHINE:~$ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/6.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-6.0.list`

`anup@u22-128-YT-MACHINE:~$ wget http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/libssl1.1_1.1.1f-1ubuntu2_amd64.deb`
`anup@u22-128-YT-MACHINE:~$ sudo dpkg -i libssl1.1_1.1.1f-1ubuntu2_amd64.deb`

`anup@u22-128-YT-MACHINE:~$ sudo apt-get update`
`anup@u22-128-YT-MACHINE:~$ sudo apt-get install -y mongodb-org`

`anup@u22-128-YT-MACHINE:~$ sudo systemctl start mongod`
`anup@u22-128-YT-MACHINE:~$ sudo systemctl enable mongod`
`anup@u22-128-YT-MACHINE:~$ sudo systemctl status mongod`

`anup@u22-128-YT-MACHINE:~$ mongod --version`
`anup@u22-128-YT-MACHINE:~$ mongosh --version`

`anup@u22-128-YT-MACHINE:~$ mongosh`

