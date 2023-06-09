# 低命令市场

这是是一个低命令市场仓库，用以展示、存放各种低命令的配置和说明。  
用户可以在这个市场搜索和安装对应的低命令。

# 使用低命令
### 安装低命令浏览器扩展
chrome应用商店搜索"低命令"进行扩展安装或者[离线下载](https://cmd.pub/crx/cmd.pub.7z)

### 安装低命令
已安装低命令浏览器扩展后，进入到例如`https://github.com/low-command/market/baidu`页面会出现`一键添加低命令`按钮，点击即可安装低命令。


# 开发低命令
### 开发和调试
1. 进入低命令管理面板点击`新增低命令`
2. 进入到普通网页按快捷键`ALT+K`运行新增的低命令看效果
3. 注意编写`readme.md`文档

# 发布到低命令市场
进入低命令管理面板，找到对应低命令导出配置JSON。  
进入低命令市场的[github页面](https://github.com/low-command/market)，clone仓库发起PR即可。  
pr分支名称规则`feat/低命令Id/版本号`，例如`feat/baidu/0.0.1`。  
所有低命令配置都放到项目路径`market/sources`下面。  
管理员审核通过后即merge分支。   



### 注意
暂不支持同名称的低命令安装。

### 低命令配置JSON字段
姓名|技能| 是否必填 | 格式 |
--|:--:|--:|--:| 
cmdId| 低命令Id | 必填 | 字符串(字母和数字)  |
cmdName| 低命令名称 | 必填 | 字符串(字母和数字) |
argList|低命令命令参数| 选填  | 数组 |
callback|低命令回调函数| 必填 | 字符串(函数) |
version| 版本号 | 必填 | 字符串(比如"0.1") |
description| 低命令描述 | 选填 |字符串 |