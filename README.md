# ProcessCommunication
This is a project to test and discover the different types of communications that can be used to communicate processes/applications

## gRPC

To use gRPC the steps are:

1. Define the service, request and response types using the protocol buffers.
2. Compile the .proto file using the protoc command (this tools needs to be previously installed). For this case the command used is:

```python -m grpc_tools.protoc -I../protos --python_out=. --pyi_out=. --grpc_python_out=. ../protos/interface.proto```

<b>Protocol buffers</b> is a mechanism for serializing structured data. It is extensible, language neutral and platform neutral mechanism. The proto compiler is called on a .proto file to generate code in various programming languages to manipulate the corresponding protocol buffer.
