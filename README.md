自动更新Openwrt,Esxi,Aruba instant ap, Synology Diskstation 证书的expect脚本。

该脚本使用前提是vps上已经安装acme.sh，并通过acme.sh申请证书。在申请证书时，添加 --renew -hook "expect UpdateAll.exp" 或者 --reloadcmd "expect UpdateAll.exp"来实现每次acme自动续期Let's encrypt证书时，自动更新其他设备的证书。

依赖expect，请自行安装。只在Ubuntu 18.04上测试过。
