命令行安装
yum install -y wget && wget -O install.sh http://www.aapanel.com/script/install_6.0_en.sh && bash install.sh forum
升级(降级)aapanel6.8.27版本（可选，当前为6.8.27版本可不执行）
wget -O /root/update6_en.sh https://download.bt.cn/install/update6_en.sh && sed -i 's/LinuxPanel_EN-${version}.zip/LinuxPanel_EN-6.8.27.zip/g' /root/update6_en.sh && bash /root/update6_en.sh && rm -rf /root/update6_en.sh
安装中文简体语言包_6.8.27(可选，需要简体执行这个)
wget -O aapanel_chinese.zip https://github.com/SanHayes/aapanel_simplified_chinese/raw/master/aapanel_simplified_chinese_6827.zip && unzip -o aapanel_chinese.zip -d /www/server/ && /etc/init.d/bt restart
安装中文繁体语言包_6.8.27(可选，需要繁体执行这个)
wget -O aapanel_chinese.zip https://github.com/SanHayes/aapanel_simplified_chinese/raw/master/aapanel_traditional_chinese_6827.zip && unzip -o aapanel_chinese.zip -d /www/server/ && /etc/init.d/bt restart
