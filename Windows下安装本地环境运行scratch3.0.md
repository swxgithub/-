#### Windows下安装本地环境运行scratch3.0

##### 1.Scoop安装

打开power shell

运行

Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://get.scoop.sh') # 或

iwr -useb get.scoop.sh | iex



##### 2.安装cmder

scoop install cmder-full    # scoop安装cmder



##### 3.安装scratch3.0

```
mkdir Scratch
cd Scratch
git clone https://github.com/llk/scratch-gui 
git clone https://github.com/llk/scratch-vm 
cd scratch-vm
npm install
npm link
npm run watch
另开一个终端
cd scratch-gui
npm install
npm link scratch-vm scratch-blocks
npm start
```

[http://localhost:8601](http://localhost:8601/)

rm -rf  文件夹名：删除非空文件夹。

