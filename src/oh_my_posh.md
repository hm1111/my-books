# Oh-my-posh
终端美化

## 安装

## 字体（可选）

### 安装字体

`oh-my-posh font install meslo`：meslo为字体名称

[参考链接](https://ohmyposh.dev/docs/installation/fonts)

### 为终端配置字体

[参考链接](https://ohmyposh.dev/docs/installation/fonts)

## 配置主题

### 创建配置文件

`New-Item -Path $PROFILE -Type File -Force`

### 修改配置文件内容
第一步：

`notepad $PROFILE`。打开配置文件

第二步：

添加`oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH/<主题文件名称>" | Invoke-Expression`到配置文件，并保存。主题文件路径可在`POSH_THEMES_PATH`环境变量中查看

第三步：

`Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine`

`. $PROFILE`。使配置文件生效


[参考链接1](https://ohmyposh.dev/docs/installation/prompt)

[参考链接2](https://ohmyposh.dev/docs/installation/customize)