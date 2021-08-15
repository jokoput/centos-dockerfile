FROM jokoput/centos:8
LABEL MAINTAINER="Joko Putranto"
RUN yum install -y zip unzip xml-common epel-release yum-utils gd gd-devel
RUN yum install -y php php-common php-opcache php-cli php-gd php-curl php-mysqli php-zip php-xml php-mbstring
#RUN yum install -y php php-common php-opcache php-mcrypt php-cli php-gd php-curl php-mysqld php-mysqli \
#        php-zip php74-php-imap php74-php-xml php-xml php74-php-zip php74-php-mbstring php-mbstring php-pecl-redis
RUN sed -e "s~;date.timezone =~date.timezone = \"UTC+7\"~g" -i /etc/php.ini
