FROM php:7.2-fpm
# RUN

RUN apt-get update && apt-get install -my wget gnupg
RUN apt-get install -y python2.7
RUN apt-get install -y python-pip
RUN apt-get install -y python3
RUN apt-get install -y python3-pip
RUN apt-get install -y graphviz
RUN pip2 install --upgrade pip
RUN pip3 install --upgrade pip

# RUN pip3 install cython
RUN pip3 install cryptography==2.8
RUN pip3 install cffi==1.13.2
RUN pip3 install cryptography==2.8
RUN pip3 install cycler==0.10.0
RUN pip3 install graphviz==0.13.2
RUN pip3 install kiwisolver==1.1.0
RUN pip3 install numpy==1.18.0
RUN pip3 install matplotlib==3.0.3
RUN pip3 install pycparser==2.19
RUN pip3 install PyNaCl==1.3.0
RUN pip3 install pyparsing==2.4.6
RUN pip3 install python-dateutil==2.8.1
RUN pip3 install six==1.13.0
RUN pip3 install stem>=1.8.0
RUN pip2 install stem>=1.8.0
RUN apt-get install -y zlib1g-dev libzip-dev
RUN docker-php-ext-install zip

RUN apt-get update
RUN apt-get install git -y
RUN git clone https://github.com/torps/torps
RUN git clone https://github.com/meda10/Tor-simulations
RUN chown -R www-data:www-data /var/www/html

# RUN chown -R www-data:www-data /var/www/html/Tor-simulations/www/html
# RUN chown -R www-data:www-data /var/www/html/torps

#RUN usermod -u 1000 www-data

# Copy existing application directory permissions
#COPY --chown=root:www-data . /var/www

# Change current user to www
# USER www-data

#COPY /Tor_Path_Simulator /Tor_Path_Simulator
#RUN chmod -R 777 /Tor_Path_Simulator
#RUN chmod -R 777 /var/www

#COPY config/mongo.ini /usr/local/etc/php/conf.d/