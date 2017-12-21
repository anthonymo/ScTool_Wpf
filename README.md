# ScTool_Wpf

ScTool is the short form of SmartContract Tools, it is a toolchain for NEO contract development.
They are all open source including two servers and one client modules. 

One module is called RemoteSharpContractBuilder which temporarily embedded in the SmartContractBrowser project.

Another server module is neo cli node which temporarily embedded in the neo-gui-nel project

We currently just deployed the API for testnet. The server is for development and will change quite frequent, we recommend you deploy your own server if you like the tools.

We use the client/server design because there ae many requests for NEO smart contract Web development tools.
The APIs are all ready for the web development tools.

## Features

This tool have two features

1. C# online compiler

![](image/pic1.png)

Copy the source code or directly write on our code editor. The avm、abi、map files will on the server if compile sucessfully.
Everyone can check the files.

This compiler use remote api, we can develop a web tool to compile c# code. 

![](image/pic2.png)

We have developed a sample.

We will eventually develop a complete web development tools for Neo smart contract.

2. Smart Contract debugging tool

Another function is to check the detail of the invoked transaction.
![](image/pic3.png)

The diagram show that our transaction.

![](image/pic4.png)

We can check the execution details by entering the transaction txid. You can download the source code if it is written by our online editor.

It contain all information you want including the values of execution stack and run-time stack, the Syscall have been used. And of course Notify Log.

3. Other Possibilties

In fact you can use this tool to develop different feature crawler to collect the unknown from NEO Blockchain. We can accurately examine every transactions based on the real time executions on the network.


## How to use

Compiler: write code -> build script

Debugging: Enter txid and see the results

GoodDay.


