# TCPA

wget https://raw.githubusercontent.com/miaocloud/TCPA/master/tcpa.sh

sh tcpa.sh


新增加速端口: 
vi  /usr/local/storage/tcpav2/start.sh 
$BINDIR/$CTLAPP access add tip $ip tport 自定义端口
 
查看是否开启成功 ：
lsmod|grep tcpa 

出现如下代码则代表启动成功：
tcpa_engine           224249  0 

卸载: 
cd /usr/local/storage/tcpav2 
sh tcpa.sh 
