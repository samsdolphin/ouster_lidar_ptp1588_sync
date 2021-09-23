首先[配置PTP主时钟](https://livox-wiki-cn.readthedocs.io/zh_CN/latest/tutorials/timestamp_sychronization.html#id14)
> git clone http://git.code.sf.net/p/linuxptp/code linuxptp \
cd linuxptp \
make -j4 \
sudo make install

编译安装后运行
> sudo ptp4l -i enp0s31f6 -l 6 -m

然后在launch file选择`TIME_FROM_PTP_1588`或者[用terminal配置](http://www.zhishibo.com/articles/4570.html)
