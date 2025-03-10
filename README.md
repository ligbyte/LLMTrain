# Android手机部署Deepseek

1、安装 termux应用

https://www.123684.com/s/usaDTd-GrIMv

2、执行
```shell
termux-setup-storage && termux-change-repo && pkg update -y && pkg upgrade -y && pkg install git cmake golang proot-distro -y && proot-distro install ubuntu && proot-distro login ubuntu
```

3、执行
```shell
git clone https://gitee.com/juneor/deepseek.git &&  .  deepseek/install.sh
```

4、执行
```shell
proot-distro login ubuntu
```

5、执行
```shell
ollama serve
```

6、开启新会话，执行
```shell
proot-distro login ubuntu
```

7、执行
```shell
ollama run deepseek-r1:1.5b
```