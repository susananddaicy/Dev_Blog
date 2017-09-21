# Dev_Blog

zsh 打开vscode命令
1. cd
2. ls -al
3. vim .zshrc
4. alias code='/Applications/Visual\ Studio\ Code.app/Contents/Resources/app/bin/code'


mac 安装nginx
1. brew install nginx
2. cd /usr/local/etc/nginx
3. nginx -v  查看版本
4. sudo nginx 启动
5. ps -ef|grep nginx  sudo kill XXX  关闭

mac 安装java
1. 下载并安装jdk  jdk1.8.0_144.jdk
2. 自己安装的jdk的目录一般在 /Library/Java/JavaVirtualMachines/jdk1.8.0_144.jdk/Contents/Home
3. 配置环境变量 (如果mac安装了zsh，需要在.zshrc添加配置，否则默认是.bashrc和.bash_profile)
    JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_40.jdk/Contents/Home;
    CLASSPATH=.:$JAVA_HOME/lib;
    export JAVA_HOME;
    export PATH=$PATH:$JAVA_HOME/bin;
4. source zshrc  让配置的环境变量生效
5. echo $JAVA_HOME  ==>  /Library/Java/JavaVirtualMachines/jdk1.8.0_40.jdk/Contents/Home
6. java -verison  查看java版本
