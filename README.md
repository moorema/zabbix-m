# zabbix-m
  - 查看tcp11种状态数量
  - ss -antp |awk '{a[$1]++}END{for(i in a)print i, a[i]}'
  - tcp.status[*],ss -antp |awk '{a[$$1]++}END{print a["'$1'"]}' #UserParameter=值
