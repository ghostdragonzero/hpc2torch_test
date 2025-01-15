# 1、创建ssh密钥
ssh-keygen -t rsa -b 2048
cat ~/.ssh/id_rsa.pub
将复制到的内容写入到 "your_copied_public_key"

# 2、将密钥上传到天数服务器
mkdir -p ~/.ssh
echo "your_copied_public_key" >> ~/.ssh/authorized_keys
chmod 600 ~/.ssh/authorized_keys
chmod 700 ~/.ssh

# 3、配置sshconfig
在vscode中ssh选项到配置文件添加如下内容

Host myserver
    HostName zibo.saas.iluvatar.com.cn
    User "youname"
    Port "youport"
    IdentityFile ~/.ssh/id_rsa