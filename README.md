<div align="center"> 
   <img height="100px" alt="logo" src="https://cdn.modrinth.com/data/wvCSIW08/a1ff154a62300a7e7813008d327a526503ad96f4.png"/> 
   <h1>VM Translation Update</h1>
</div> 

## 功能
1. 对比最新版汉化版本号与本地配置文件中的版本号，在汉化发布新版本时会在游戏里通知玩家去下载更新。
2. 默认每25分钟在聊天栏发送一条知识。内容包括但不限于汉化组冷知识，汉字易错读音和MC冷知识等。
3. 每次启动时自动下载VM汉化组通用模组汉化资源包。
4. 如果玩家已经下载资源包且发生错误未启用，会在聊天框提示玩家在选项->资源包中手动启用。
5. 如果玩家名是Zi__Min，会在每次进入世界时发送`欢迎来到籽岷的Minecraft游戏世界！`，且称呼改为岷叔。
6. 自动修改游戏语言，当安装Stenographer模组后不修改。

## 使用与配置文件

**发布汉化时，请特别注意。在汉化更新时改一下模组配置里的版本号！**

模组会在config文件夹创建名为`vmtranslationupdate`的配置文件（1.12.2后缀是.cfg，其他版本为.toml），共有7个配置选项。
1. 更新检测链接。例如`https://vmct-cn.top/modpacks/sb3/update.txt`，会读取txt的内容。必须为UTF-8编码且可以直接打开的直链。
2. 提示玩家下载的链接。例如`https://vmct-cn.top/modpacks/sb3/`，会在聊天栏展示。
3. 获取知识内容的链接。例如`https://vmct-cn.top/tips.txt`会读取txt的内容，必须是UTF-8编码且可以直接打开的直链。一行一句，每次会随机选择一行的内容发送在聊天栏。
4. 整合包翻译版本。例如第一版。需要发布时改的就是这个。
5. 发送知识的时间间隔（分钟），默认25分钟一次。
6. 自动下载资源包的链接。例如`https://cdn.modrinth.com/data/IDWIdXwS/versions/xCpjJgHS/VM汉化组模组汉化包1.18`。注：链接需要删除最后的.zip，模组会自己加上。
7. 资源包的文件名，例如`VM汉化组模组汉化包1.18`。
--- 
 ## 支持版本
 - [x] Forge
     - [x] 1.12.2
     - [x] 1.16.5
     - [x] 1.18.x
     - [x] 1.19.x
     - [x] 1.20 - 1.20.2
 - [x] Fabric
     - [x] 1.16.5
     - [x] 1.18.x
     - [x] 1.19.x
     - [x] 1.20 - 1.20.2
 - [x] Neoforge
     - [x] 1.20.2

## 其他
特别感谢TexTrue跨加载器重构，以及Lichiiiiiii修复部分bug！
许可证使用MIT协议
