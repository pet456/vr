# VR example from three.js

For building from scratch:
1. Initialize empty node project with invoking `npm init`
1. Then add three.js library by invoking `npm install three`

Before connecting VR helm to PC check launch http-server.
At terminal execute: `npx http-server .`

If VR helm require https protocol then generate `key.pem` and `cert.pem`:
`openssl req -newkey rsa:2048 -new -nodes -x509 -days 3650 -keyout key.pem -out cert.pem`

After you can start http server with enabling SSL:
`http-server -S -C cert.pem -o` or `npx http-server -S -C cert.pem -o`