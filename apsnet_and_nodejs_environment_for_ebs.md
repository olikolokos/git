# Asp.net and Node environment for EBS

#### There’s a few things you must know before we start.




*The asp.net environment will be avaliable for 173 days, because it is a trial version.*


*You'll have to use your domain credentials to  access IIS server and SQL server (Mail Helpdesk asking for permissions).*


*you're not allowed to use any kind of piracy.*

#### How to access the server.

You can use Windows built-in software for remote desktop access, or you can even download a express version of SQL management tool and IIS remote management tool, the servername is : POMPEII-SERVER or you can access it by the ip address: 192.168.150.27



* 
[IIS management Rremote administration](http://www.microsoft.com/en-us/download/details.aspx?id=41177)


* 
[Sql Server managemant Studio Express](http://www.microsoft.com/en-us/download/details.aspx?id=8961)

####  What This server has?

This server has a SQL server, IIS server, GIT and net framework4.5.

#### What about the linux server?

A Mysql server, an Apache server , php modules, NodeJS modules, GIT , Docker and MongoDB.

#### How do i Access this server?

to access this server you'll have to  mail helpdesk with your public  ssh key, if you are using **Putty** ([Putty Download](http://the.earth.li/~sgtatham/putty/latest/x86/putty.exe)) you'll have to follow a few steps:

First of all download [PuttyGen](http://the.earth.li/~sgtatham/putty/latest/x86/puttygen.exe)
Execute generate a 1024 bits key like the image below

![](https://fbcdn-sphotos-g-a.akamaihd.net/hphotos-ak-xpa1/v/t1.0-9/10923627_921873291178791_5184804320464515594_n.jpg?oh=6819f19ec264efe57c2203c8883e875b&oe=5522539F&__gda__=1432331303_25cc43c0ae4cfffb183cb52a09d7d9f8)

After generating the public, open Putty software and at the ssh section save you private and add it to Putty.



![](https://fbcdn-sphotos-d-a.akamaihd.net/hphotos-ak-xpf1/v/t1.0-9/10406512_921878334511620_6985504713214886103_n.jpg?oh=4832f771a3177c0bb767d53444074b89&oe=5563EF8B&__gda__=1428469217_b31d01f4f9c9f085861560a418a5e921)


And then add  autologin "root" to "Connections > Data > Auto-login username".



![](https://scontent-a-gru.xx.fbcdn.net/hphotos-prn2/v/t1.0-9/10931333_921873294512124_2546614696336870759_n.jpg?oh=b5a3fbc4c48f04af8120c6c30193914e&oe=55281DED)

For the final step, add the ip address or the servername to "HostName" field(22 is the default port).


![](https://scontent-b-gru.xx.fbcdn.net/hphotos-xpf1/v/t1.0-9/10456036_921025871263533_6888076615864975161_n.jpg?oh=f12067db48196a226e368039d5d0e987&oe=55667D7B)

Then click open and you are set.

![](https://fbcdn-sphotos-d-a.akamaihd.net/hphotos-ak-xap1/v/t1.0-9/p75x225/10923234_920856041280516_3608805919538511181_n.jpg?oh=1bbb9b32fd864dfebaafc52752bd8bda&oe=555CA23D&__gda__=1428610580_806b8f695c971fac24e8f8229861fa3d)

Now if you are using Linux you'll use a cli ssh-client.
First install the ssh software:

```sudo apt-get install ssh```


then generate your rsa public key by typing:

```ssh-keygen -t rsa -C "your.mail@bravi.com.br"```

Copy the content of .ssh/id_rsa.pub:

```cat ~/.ssh/id_rsa.pub```

And send to helpdesk, when helpdesk confirm your ssh key you can access the server by typing:

```ssh root@ebs-node.bravi.com.br```

Or

```ssh root@192.168.150.210```











    






