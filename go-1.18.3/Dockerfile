FROM registry.cn-shanghai.aliyuncs.com/eldenring/lichking:ubuntu-20.04-utf8
RUN apt update && apt install -y build-essential curl net-tools wget && wget -P /usr/local https://golang.org/dl/go1.18.3.linux-amd64.tar.gz && tar zxvf /usr/local/go1.18.3.linux-amd64.tar.gz -C /usr/local && rm -f /usr/local/go1.18.3.linux-amd64.tar.gz
ENV PATH '/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/go/bin'
WORKDIR /app