FROM registry.cn-shanghai.aliyuncs.com/eldenring/lichking:ubuntu-20.04-utf8
RUN apt update && apt install -y curl net-tools wget build-essential zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev libssl-dev libreadline-dev libffi-dev libsqlite3-dev 
RUN wget -P /usr/local/src https://www.python.org/ftp/python/3.7.9/Python-3.7.9.tar.xz && tar Jxvf /usr/local/src/Python-3.7.9.tar.xz -C /usr/local/src && rm -f /usr/local/src/Python-3.7.9.tar.xz && cd /usr/local/src/Python-3.7.9 && ./configure --prefix=/usr/local/python3 --with-ssl && make && make install
ENV PATH '/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/python3/bin'
WORKDIR /app