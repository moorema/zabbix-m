# zabbix-m
  - 查看tcp11种状态数量
  - ss -antp |awk '{a[$1]++}END{for(i in a)print i, a[i]}'
