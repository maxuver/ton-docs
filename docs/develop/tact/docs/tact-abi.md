# Tact ABI 

### What is ABI?
The Application Binary Interface (ABI) is a specification for how a contract interface should be encoded in TON's data format, the TON Virtual Machine (TVM) bytecode. 

Since this bytecode is not human readable, it requires interpretation to be understood. ABI allows anyone writing a smart contract to be able to communicate between a web application written in a high-level language like Javascript and the bytecode that the EVM understands. It defines the data types and functions that can be called on a contract, as well as the encoding of the data that is passed to and from the contract. The ABI is important because it allows users to interact with smart contracts in a predictable and standard way, regardless of the programming language that was used to write the contract. 

It also allows tools and libraries to be built that can parse and generate the data required to call contract functions, making it easier for developers to build applications that interact with smart contracts.

### Processing ABI in the TACT
ABI acts as a function selector, defining the specific methods that can be called to a smart contract for execution. These specific methods and their connected data types are listed in a generated JSON RPC file. Tact compiler do this by default for each contract, here is example of ABI for counter.contract:

![Tact ABI template](/img/docs/tact-abi-example.png?raw=true)

### ABI use case

![Tact ABI](/img/docs/tact-abi.png?raw=true)
