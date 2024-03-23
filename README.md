# VScode in BROWSER 
###### --by Hopen

## But why?

VScode stands for Visual Studio Code, which is a cross-platform editor launched by Microsoft, which can run on windows, Linux, IOS and other platforms, and can become a compiler by installing some plug-ins. With support for C++, Python, Java, C#, Go, and more, VSCode is powerful, plug-in-rich, and extremely fast, making it worth every developer to try!

**But!!**

It's quite difficult to install VSCode on **Android,or termux** and hard to **connect multiple devices**, so I made this script to help you

***and***

it also solve the problem of arm to Andriod system matching issue and multiple devices  

Here's the preview of the script

![preview](https://cdn.luogu.com.cn/upload/image_hosting/1ickgpqe.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/1kie78iu.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/1jc4x561.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/vci7bs0c.png)

## download steps
*******************************

-  start termux (zerotermux)
-  agree all
- input these:(one by one)
- ***for Chinese make sure github.com is working***

github isn't stable in China
```    
apt updat && apt upgrade && pkg install git -y

git clone https://github.com/hopen-hub/server-hopen.git

cd server-hopen/ && chmod +x autodownload.sh

./autodownload.sh
```


and wait

.....

It may take some time......
remember don't leave!

![](https://cdn.luogu.com.cn/upload/image_hosting/1r6z9dd2.png)

 - When it's done ,you will see something just like this

![](https://cdn.luogu.com.cn/upload/image_hosting/ms3l5a9z.png)

## configrations

- then you can restart termux(zerotermux)
- input `vim ~/.config/code-server/config.yaml`
you will see this:

![](https://cdn.luogu.com.cn/upload/image_hosting/dw8ty44v.png)

`bind-addr: `is you code-server local address

if you want multiple-devices function,press letter `i` 

and change `127.0.0.1:8080` to 
`0.0.0.0:8080`

and change `password: *****` to your password

then press `Esc` and `:wq` to save and quit

## local uasge

now you can start vscode by input `code-server` in termux
then go to a browser and input 
`localhost:8080` 

## connect to multiple devices

- check your Ip address

- running code-server in your local termux 


- onpen a browser in another device and input `(your ip adress):8080`

and input your password

***and here you go!***
