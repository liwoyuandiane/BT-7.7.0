# BT-7.7.0
宝塔面板退回7.7.0文件

#使用步骤
```shell
cd /root/
wget https://github.com/liwoyuandiane/BT-7.7.0/blob/main/LinuxPanel-7.7.0.zip
unzip LinuxPanel-7.7.0.zip
cd /root/panel
bash update.sh
rm -f /www/server/panel/data/bind.pl
```shell
