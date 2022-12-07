# BT-7.7.0
宝塔面板退回7.7.0文件

## 使用步骤
```shell
cd /root/
wget https://github.com/liwoyuandiane/BT-7.7.0/blob/main/LinuxPanel-7.7.0.zip
unzip LinuxPanel-7.7.0.zip
cd /root/panel
bash update.sh
rm -f /www/server/panel/data/bind.pl
```


## 加速链接
```shell
cd /root/
wget https://liwoyuandianer-my.sharepoint.com/personal/liwoyuandianer_liwoyuandianer_onmicrosoft_com/_layouts/52/download.aspx?share=ETKEa7gximdMoGZat3bybUwB686iLqyv8Ynw7v0rVV5I8A -O /root/LinuxPanel-7.7.0.zip
unzip LinuxPanel-7.7.0.zip
cd /root/panel
bash update.sh
rm -f /www/server/panel/data/bind.pl
```
## 官方链接
```shell
cd /root/
wget http://download.bt.cn/install/update/LinuxPanel-7.7.0.zip
unzip LinuxPanel-7.7.0.zip
cd /root/LinuxPanel-7.7.0/panel
bash update.sh
rm -f /www/server/panel/data/bind.pl
```

### 临时屏蔽强制绑定手机
```shell
sed -i "s|bind_user == 'True'|bind_user == 'XXXX'|" /www/server/panel/BTPanel/static/js/index.js

#如果需要恢复……
sed -i "s|if (bind_user == 'REMOVED') {|if (bind_user == 'True') {|g" /www/server/panel/BTPanel/static/js/index.js
```
