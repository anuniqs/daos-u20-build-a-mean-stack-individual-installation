### Pre-requisites,
 
`anup@u22-128-YT-MACHINE:~$ sudo apt install build-essential`

### MongoDB,

https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-ubuntu/

`anup@u22-128-YT-MACHINE:~$ sudo apt-get install gnupg`

`anup@u22-128-YT-MACHINE:~$ wget -qO - https://www.mongodb.org/static/pgp/server-6.0.asc | sudo apt-key add -`

`anup@u22-128-YT-MACHINE:~$ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/6.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-6.0.list`

<br>

`anup@u22-128-YT-MACHINE:~$ wget http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/libssl1.1_1.1.1f-1ubuntu2_amd64.deb`

`anup@u22-128-YT-MACHINE:~$ sudo dpkg -i libssl1.1_1.1.1f-1ubuntu2_amd64.deb`

<br>

`anup@u22-128-YT-MACHINE:~$ sudo apt-get update`

`anup@u22-128-YT-MACHINE:~$ sudo apt-get install -y mongodb-org`

<br>

`anup@u22-128-YT-MACHINE:~$ sudo systemctl start mongod`

`anup@u22-128-YT-MACHINE:~$ sudo systemctl enable mongod`

`anup@u22-128-YT-MACHINE:~$ sudo systemctl status mongod`

<br>

`anup@u22-128-YT-MACHINE:~$ mongod --version`

`anup@u22-128-YT-MACHINE:~$ mongosh --version`

<br>

`anup@u22-128-YT-MACHINE:~$ mongosh`

<br>
<br>
<br>

### Node.js,

https://github.com/nodesource/distributions/blob/master/README.md#debinstall

`anup@u22-128-YT-MACHINE:~$ sudo apt-get install curl`

<br>

`anup@u22-128-YT-MACHINE:~$ curl -sL https://deb.nodesource.com/setup_16.x | sudo -E bash -`

`anup@u22-128-YT-MACHINE:~$ sudo apt-get install -y nodejs`

<br>

`anup@u22-128-YT-MACHINE:~$ node --version`

`anup@u22-128-YT-MACHINE:~$ npm --version`

`anup@u22-128-YT-MACHINE:~$ npx --version`

<br>

`anup@u22-128-YT-MACHINE:~$ sudo npm install -g express-generator`

`anup@u22-128-YT-MACHINE:~$ express --version`

<br>

`anup@u22-128-YT-MACHINE:~$ express --view=pug myapp`

`anup@u22-128-YT-MACHINE:~$ cd myapp/`

`anup@u22-128-YT-MACHINE:~/myapp$ npm install`

`anup@u22-128-YT-MACHINE:~/myapp$ ls -ltr`

`anup@u22-128-YT-MACHINE:~/myapp$ sudo apt-get install tree`

`anup@u22-128-YT-MACHINE:~/myapp$ tree`

<br>

`anup@u22-128-YT-MACHINE:~/myapp/bin$ cat www `

<br>

`anup@u22-128-YT-MACHINE:~/myapp$ DEBUG=myapp:* npm start`

<br>

http://192.168.56.128:3000/

<br>
<br>
<br>

### Express.js,

https://expressjs.com/

`anup@u22-128-YT-MACHINE:~$ sudo npm install -g express`

`anup@u22-128-YT-MACHINE:~$ sudo npm install -g npm@9.2.0`

<br>

`anup@u22-128-YT-MACHINE:~$ sudo npm view express version`

<br>

`anup@u22-128-YT-MACHINE:~$ mkdir myproject`

`anup@u22-128-YT-MACHINE:~$ cd myproject`

`anup@u22-128-YT-MACHINE:~/myproject$ npm init -y`

`anup@u22-128-YT-MACHINE:~/myproject$ npm install express`

<br>

`anup@u22-128-YT-MACHINE:~/myproject$ sudo nano app.js`


    const express = require('express')
    
    const app = express()
    
    const port = 3001
    
    
    
    app.get('/', (req, res) => {
    
        res.send('Hello There!')
    
    })
    
    
    
    app.listen(port, () => {
    
        console.log(`Example app listening at http://localhost:${port}`)
    
    })


`anup@u22-128-YT-MACHINE:~/myproject$ node app.js`

http://192.168.56.128:3001/

http://localhost:3001

<br>
<br>
<br>

### AngularJS,

`anup@u22-128-YT-MACHINE:~$ sudo npm install -g @angular/cli`

`anup@u22-128-YT-MACHINE:~$ ng version | ng v `

`anup@u22-128-YT-MACHINE:~$ ng new angular-tour-of-heroes`

`anup@u22-128-YT-MACHINE:~$ cd angular-tour-of-heroes/`

`anup@u22-128-YT-MACHINE:~/angular-tour-of-heroes$ ng serve --open`

http://localhost:4200
