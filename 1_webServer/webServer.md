# An example of a web server 
1. create folder  'webServer';
2. cd webServer ;
3. put the code into a file called websever.js;
``` 
const http = require('http');

const hostname = '127.0.0.1';
const port = 3000;

const server = http.createServer((req, res) => {
  res.statusCode = 200;
  res.setHeader('Content-Type', 'text/plain');
  res.end('Hello World\n');
});

server.listen(port, hostname, () => {
  console.log(`Server running at http://${hostname}:${port}/`);
});
```
4. execute webserver.js with nodejs ;
```
$ node example.js
Server running at http://127.0.0.1:3000/
```