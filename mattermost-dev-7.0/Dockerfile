FROM registry.cn-shanghai.aliyuncs.com/eldenring/lichking:ubuntu-20.04-utf8
RUN apt update && apt install -y tree iputils-ping build-essential gcc nasm libpng-dev curl net-tools wget unzip
COPY go1.18.8.linux-amd64.tar.gz /usr/local/go1.18.8.linux-amd64.tar.gz
COPY node-v16.10.0-linux-x64.tar.xz /usr/local/node-v16.10.0-linux-x64.tar.xz 
COPY node_modules.tar.gz /var/node_modules.tar.gz
RUN tar zxvf /usr/local/go1.18.8.linux-amd64.tar.gz -C /usr/local && rm -f /usr/local/go1.18.8.linux-amd64.tar.gz && tar Jxvf /usr/local/node-v16.10.0-linux-x64.tar.xz -C /usr/local && rm -f /usr/local/node-v16.10.0-linux-x64.tar.xz && tar zxvf /var/node_modules.tar.gz -C /var && rm -rf /var/node_modules.tar.gz
ENV PATH '/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/node-v16.10.0-linux-x64/bin:/usr/local/go/bin'
WORKDIR /app
