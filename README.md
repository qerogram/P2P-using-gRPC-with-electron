# P2P-using-gRPC-with-electron

# server

## Execute
1. docker build . -t grpc_server
2. docker run -v ./files:/app/files -p 8282:8282 -itd grpc_server 

# client

##  Execute
1. Execute Command - ```npm install``` on the root dir.
2. Execute Command - ```npm install``` on the src dir.
3. Execute Command - ```npm start``` on the root dir.

## Compile
1. Execute Command - ```npm install``` on the root dir.
2. Execute Command - ```npm install``` on the src dir.
3. Execute Command - ```npx electron-builder build --windows``` on the root dir.
4. we find the binary in dist/win-unpacked/client.exe
5. we make a 'addr.txt' in the path(dist/win-unpacked/addr.txt). And we write the gRPC Server Address(ex, 192.168.0.231:8282)