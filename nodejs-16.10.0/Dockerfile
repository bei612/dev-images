FROM registry.cn-shanghai.aliyuncs.com/eldenring/lichking:ubuntu-20.04-utf8
RUN apt update && apt install -y curl net-tools wget xz-utils && wget -P /usr/local https://nodejs.org/dist/v16.10.0/node-v16.10.0-linux-x64.tar.xz && tar Jxvf /usr/local/node-v16.10.0-linux-x64.tar.xz -C /usr/local && rm -f /usr/local/node-v16.10.0-linux-x64.tar.xz
ENV PATH '/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/node-v16.10.0-linux-x64/bin'
WORKDIR /app