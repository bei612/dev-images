FROM registry.cn-shanghai.aliyuncs.com/eldenring/lichking:ubuntu-20.04-utf8
RUN apt update && apt install -y tree iputils-ping build-essential gcc nasm libpng-dev curl net-tools wget unzip
RUN wget -P /usr/local https://golang.org/dl/go1.18.3.linux-amd64.tar.gz && tar zxvf /usr/local/go1.18.3.linux-amd64.tar.gz -C /usr/local && rm -f /usr/local/go1.18.3.linux-amd64.tar.gz
RUN wget -P /usr/local https://nodejs.org/dist/v16.15.1/node-v16.15.1-linux-x64.tar.xz && tar Jxvf /usr/local/node-v16.15.1-linux-x64.tar.xz -C /usr/local && rm -f /usr/local/node-v16.15.1-linux-x64.tar.xz 
ENV PATH '/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/node-v16.15.1-linux-x64/bin:/usr/local/go/bin'
WORKDIR /app