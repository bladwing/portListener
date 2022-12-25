# Port Listener C#

## How to use?


Install required **.NET 7.0 SDK** [package](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/sdk-7.0.100-windows-x64-installer) 


Run - **Windows PowerShell**

Go to workdirectory 


```
c:/"workingdirectory"

git clone git@github.com:bladwing/portListener.git

cd portListener

dotnet run

```

PowerShell will get message - 

`Waiting for a connection...`


After that we have to check our Listener

Download [Hercules SETUP utility ](https://www.hw-group.com/software/hercules-setup-utility)

Run application / Go to TCP Client TAB / change IP && Port / Connect (default in Listener: ip 127.0.0.1  port: 5000)

you get message in PowerShell -

`Waiting for a connection... Connected!`

![](https://i.imgur.com/csVLimW.png)

You can sent some text data 


![](https://i.imgur.com/KmYcpaw.png)



Note: if you need to change ip and port in Listener: Open in VS code - Program.cs and change value for 

```
Int32 port = 5000;
IPAddress localAddr = IPAddress.Parse("127.0.0.1");
```

![](https://i.imgur.com/yM9d5wD.png)














