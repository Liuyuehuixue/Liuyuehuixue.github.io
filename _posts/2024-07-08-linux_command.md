---
layout: post
title: linux base commands
date: 2024-07-08 22:28 +0800
categories: [linux, command]
tag: linux, command
---

### linux base command

#### service

```linux
# 服务xxx启动 重启 停止
sudo service xxx start
sudo service xxx restart
sudo service xxx stop

# 查看服务xxx状态
systemctl status xxx
```

####  log 重定向

```linux
# 导出 2024年1月1日 14:00 到 16:00 之间，服务 myservice 的所有包含 "ERROR" 关键字的错误日志

journalctl -u myservice --since "2023-01-01 14:00:00" --until "2023-01-01 16:00:00" | grep "ERROR" > /path/to/exported_filtered_log.txt

```


