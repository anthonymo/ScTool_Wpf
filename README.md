# ScTool_Wpf

ScTool is the short form of SmartContract Tools, it is a toolchain for NEO contract development.
They are all open source that include two server and one client modules. 

ScTool 是 SmartContract Tools 的简写，是一套NEO智能合约调测工具。
嗯，他是一套工具。包含两组服务器和前端，全部都开源。

One module is called RemoteSharpContractBuilder which temporarily embedded in the SmartContractBrowser project.

一组服务器叫做RemoteSharpContractBuilder,暂时存放在SmartContractBrowser 项目中。

Another server module is aneo cli node which temporarily embedded in the neo-gui-nel project

另一组服务器是一个定制的 neo cli 节点,暂时存放在neo-gui-nel 项目中。

We currently just depployed the API for testnet. The server is for developerment and will change quite frequent, we recommend you deploy your own server if you like the tools.

目前我们只部署了TestNet的服务API，由于我们的服务器是开发使用，经常会做各种操作。如果你喜欢这套工具，我们建议你自己部署服务。

We use the client/server design because there ae many requests for a Web development tools.
The API are all ready for the web development tools.

我们直接采用了前后端分离的设计，是因为请求开发Web工具集呼声很的高。
我们已经准备好为Web开发工具集的API。

## 功能

This tools have two features
这套工具目前主要有两个功能

1.C# online compiler
1.C# online编译器

![](image/pic1.png)
Copy the source code or directly write on our code editor. The avm、abi、map fiel will on the server if compile sucessfully.
Everyone can check the files.

将代码复制进来，或者在这里编写。若生成成功，你的源码、avm、abi文件、map文件 会被保存在服务器上。
任何人均可查看。

This compiler use remote api,so we can develop a web tool to compile c# code. 

这个编译器基于远程API工作，所以他可以开发一个Web版本
![](image/pic2.png)
We develop a sample.

We wil eventually develop a complete web development tools.
最终，我们会提供一整套的Web开发工具。

2. Smart Contract debugging tool
2.智能合约交易调试工具

Another function is to check the detail of teh invoked transaction.
另一个功能是针对一个具体的交易，查看他的执行细节
![](image/pic3.png)
The diagram show that we send a transaction.
如图我们刚刚发起了一笔交易
![](image/pic4.png)

We can check the execution details by entering the transaction txid. 
YOu can download the source code if it is written by our online editor.
然后在调试工具中输入交易ID即可查询交易执行的细节。
如果调用链中包含你用我们的C#online编译器编译的合约，我们还能自动帮你下载到源码，并对应。

It contain all information you want. The value of execution stack and run-time stack. What Syscall have been used.
And of course Notify Log.

这里有你需要的一切信息。
执行栈和计算栈上的值在每一步的时候的情况。
有哪些Syscall被调用。
Notify Log 这些都不在话下。

3. Other Possibilties
3.其他可能性

In fact you can use this tool to develop feature crawler, collect the unkown from NEO Blockchain.
We can accuratly examine every transaction based on the real time execution of transactions.

实际上，你也可以利用这套调试工具去开发特色的爬虫，收集NEO区块链上不为人所知的秘密。
我们可以准确的判定一个智能合约交易的行为，完全基于链上真实执行情况。

How to use
## 使用方法

Compiler: write code -> build script
编译功能的使用方法：写代码->按编译按钮->看到结果并自动保存在服务器

Debugging: Enter txid and see the results
调试功能的使用方法：输入txid->按load按钮->看结果

GoodDay.


