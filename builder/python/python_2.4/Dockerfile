FROM bradrydzewski/base
WORKDIR /home/ubuntu
USER ubuntu
ADD python.sh /etc/drone.d/

RUN sudo easy_install virtualenv==1.7.2 && \
    sudo add-apt-repository --yes ppa:fkrull/deadsnakes && \
    sudo apt-get update && sudo apt-get install && sudo apt-get install python2.4 python2.4-dev && \
    mkdir -p /home/ubuntu/virtualenv && \
    virtualenv --python=/usr/bin/python2.4 /home/ubuntu/virtualenv/python2.4 --use-distribute
