# How it works
<image src = "working.png">



## Installation

build this image as

```bash
"docker build -t wsapp ."
```
next run 
```bash
docker-compose up
```
## Usage
open a browser console and type this
```bash
let ws = new WebSocket("ws://localhost:8080");
ws.onmessage = message => console.log(`Received: ${message.data}`);
ws.send("Hello! I'm client")
```
open multiple console windows to simulate multiple clients

## License

[MIT](https://choosealicense.com/licenses/mit/)
