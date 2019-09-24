FROM phplist/phplist:3.4.1
WORKDIR /root/
RUN git clone https://github.com/phpList/phplist3
RUN rm -Rf /var/www/phpList3/public_html/lists
CMD cp -rf ~/phplist3/public_html/lists /var/www/phpList3/public_html/
