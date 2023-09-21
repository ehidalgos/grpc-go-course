# Differences between HTTP/1 and HTTP/2

## HTTP/1

* TCP Connection per request
* Plaintext headers
* Request / Response

## HTTP/2

* One TCP Connection
* Server push
* Multiplexing

### GRPC

* Payload binary
* SSL
* Less chatter
* Less bandwidth
* More security

# Types of API in gRPC

* Unary: clients will send one requests and the server will return one response.
* Server streaming: enabled by HTTP/2, the clients will send one request and the server can return one or more responses
  depending on the need.
* Client streaming: the clients will send one or more request and the server returns one response.
* Bidirectional streaming: the client can send multiple requests and the server can return multiple answers.

# Scalability in gRPC

* Server: Async
* Client: Async or Blocking
* Google: 10 Billions requests/sec

# Security in gRPC (SSL)

* Schema based serialization
* Easy SSL certificates initialization
* Interceptors for Auth

# gRPC vs REST

## gRPC

* Protocol Buffers
* HTTP 2
* Streaming
* Bidirectional
* Free design

## REST

* JSON
* HTTP 1
* Unary
* Client -> Server
* GET/POST/UPDATE/DELETE

# Why use gRPC

* Code generation
* More secure
* Streaming
* API oriented
