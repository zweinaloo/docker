# DOCKER-VERSION 1.8.1

FORM centos:6.4

#Enable EPEL for Node.js
RUN rpm -Uvh http://download.fedoraproject.org/pub/epel/6/i386/epel-release-6-8.noarch.rpm
#Install Node.js and npm
RUN yum install -y npm

#Bundle app source 
ADD . /src

RUN cd /src; npm install

EXPOSE 9090

CMD ["node","/src/index.js"]

