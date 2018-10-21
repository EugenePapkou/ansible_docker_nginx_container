FROM centos
LABEL maintainer="Eugene Papkou"
RUN rpm -Uvh http://nginx.org/packages/centos/7/noarch/RPMS/nginx-release-centos-7-0.el7.ngx.noarch.rpm && \
yum -y install epel-release && yum -y install nginx && echo "Made by $(whoami) user." > /usr/share/nginx/html/index.html
EXPOSE 80
ENTRYPOINT ["nginx"]
CMD ["-g", "daemon off;"]

