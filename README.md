## 核酸自动提交脚本
> 原理非常简单，主要就是利用自动化测试工具来完成网页填表

### Quick Start

------------

#### 环境要求
- 至少 15G 硬盘空间
- 至少 4G 内存
- VMware 16.x 及以上版本

#### 1.安装虚拟机
- 首先安装VMware 16.2 版本（如果已安装可以跳过），这里提供第三方下载地址: [第三方下载地址](http://www.123pan.com/s/HQeA-aX1Sh "第三方下载地址")，密钥：[密钥](https://www.ghxi.com/vmware15.html "密钥")

- 然后下载配置好的虚拟机，下载地址为：[http://pan.shanghaitech.edu.cn/cloudservice/outerLink/decode?c3Vnb24xNjY4NzcyMDUwMTcyc3Vnb24=](http://pan.shanghaitech.edu.cn/cloudservice/outerLink/decode?c3Vnb24xNjY4NzcyMDUwMTcyc3Vnb24= "http://pan.shanghaitech.edu.cn/cloudservice/outerLink/decode?c3Vnb24xNjY4NzcyMDUwMTcyc3Vnb24=")

- 解压压缩包，打开.vmx后缀的虚拟机文件。若vmware弹出提示，点击"我已复制该虚拟机"

#### 2.配置手机模拟器
- 将虚拟机开机，点击其中的" 手机模拟器" 快捷方式， 开启手机模拟器
- 待手机开机后，点击右上角齿轮设置，在 **手机-开启网络连接** 设置中，将网络连接**关闭**
- 打开随申办市民云APP，初次打开时APP会要求地理位置信息，**点击拒绝**
- 在下方栏目找到 **我的**，转移至登录页面
- 输入你的随申办账号和密码。（如果不记得密码可点击：[随申办忘记密码](https://zwdtuser.sh.gov.cn/uc/forget/RetrievePassword.html "随申办忘记密码")）
- 输入完账号密码后，进入模拟器右上角齿轮设置，将网络连接**打开**，并登录你的账号
- 当账号成功登陆后，回到随申办APP首页，当其弹出强制更新窗口时，**请不要更新！**
- 在模拟器中划出 近期任务（就是任务栏），直接关闭随申办APP
- 进入模拟器右上角齿轮设置，将网络连接**关闭**，并打开随申办APP
- 直到进入首页无强制更新弹窗，点击**核酸查询**
- 进入模拟器右上角齿轮设置，将网络连接**开启**，等待一段时间后返回随申办APP首页
- 停留在随申办APP首页，确保首页中有**核酸查询**模块且无强制更新弹窗，请不要做其他的操作

#### 3.运行脚本文件
- 双击打开 ./脚本/自动脚本.py ，在代码顶端可以见到有hesuan_date,user_name,user_password需要进行配置
- 配置完成后直接运行脚本即可

#### 4.保持脚本运行
- 将虚拟机 保持在后台运行 即可
- 在你设定的核酸日时，脚本将会自动将探测到的核酸结果上交到问卷中。

### 常见问题

------------

#### 1.随申办一直弹出强行更新窗口
- 见步骤 2.配置手机模拟器，请确保网络已经关闭，以及随申办APP在 近期任务 中 被彻底关闭

#### 2.随申办闪退
- 说明你已经更新了最新的随申办APP，请在以下链接中重新下载app，并将其安装在手机模拟器中
[随申办下载连接](http://pan.shanghaitech.edu.cn/cloudservice/outerLink/decode?c3Vnb24xNjY4Nzc0NzMxMTU0c3Vnb24= "随申办下载连接")

#### 2.一直显示 "连接出现故障，一分钟后重连" 报错
- 请确保随申办位于首页；随申办首页中有核酸查询栏目；随申办APP无强制升级及其他弹窗。

#### 2.显示 "问卷提交部分有bug，请及时修复" 报错
- 我的问题，联系我尽快修复bug
