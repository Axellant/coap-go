# Lobaro CoAP GoLang adapter

[Lobaro CoAP](https://gitlab.com/lobaro/lobaro-coap) provides a highly portable CoAP stack for Client and Server running on almost any hardware.

The **GoLang adapter** uses cgo to provide a CoAP stack based on the code of Lobaro CoAP. It can be used for **testing the stack on a PC** and to **write server applications in go** that can handle CoAP connections.

## Getting Started

### Prerequisite 
To build the project you need a C compiler and the matching [Go](https://golang.org/dl/) toolkit installed. 

For Windows you can use [MinGW](http://www.mingw.org/) to install the gcc. 

When you have a 32 bit C compiler make sure you also use 32 bit Go. Else cgo will not be able to compile the C code.

### Install the code

```
go get -u gitlab.com/lobaro/lobaro-coap-go
```

Execute tests
```
go test gitlab.com/lobaro/lobaro-coap-go
```

To use the library in your project, just import
```
import "gitlab.com/lobaro/lobaro-coap-go/coap"
```
