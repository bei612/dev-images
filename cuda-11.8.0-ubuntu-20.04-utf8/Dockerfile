FROM nvidia/cuda:11.8.0-devel-ubuntu22.04
RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y software-properties-common && add-apt-repository ppa:git-core/ppa
RUN apt-get update && apt-get install -y git locales wget vim && locale-gen en_US.UTF-8 
ENV LC_ALL 'en_US.UTF-8'