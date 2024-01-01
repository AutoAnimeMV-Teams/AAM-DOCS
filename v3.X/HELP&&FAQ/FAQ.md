`最后更新时间：2023.12.29-14:05`
***
# 目录
+ [常见问题](/DOCS.md/##常见问题)
    - pip安装出现问题
    - 群晖NAS使用Python出现奇怪的问题


# 常见问题

## 1）pip安装出现问题
*   如果您直接使用pip进行install遇到 `❗Fatal error in launcher: Unable to create process using pip问题`
请使用`python3 -m pip install` 尝试安装

## 2）群晖NAS使用Python出现奇怪的问题
* 在群晖NAS中，套件中心安装的`🐍python3`环境可能出现奇奇怪怪的问题，请使用第三方套件源(第三方源需要手动为`🐍python3`创建软连接至/usr/local/bin/python3)

## 3）下载完后出现权限错误
* 如果是您手动创建的目录后出现此问题，请删除目录让脚本自动创建

## 4）Log 保存位置在哪？
* 默认情况下,Log文件会保存在传入的`保存路径`下,当无法访问此路径时,Log保存在工具目录下

## 5） Api功能
> Api功能默认开启,在一般情况下我们不建议关闭
* 当您同时启用 `BGMAPI` 和 `TMDBAPI`时,如果匹配出的是中文,将会优先交给 `BGMAPI` 识别,如果有返回值再把返回值交给 `TMDBAPI` 识别,如果没有则让 `TMDBAPI` 识别原匹配