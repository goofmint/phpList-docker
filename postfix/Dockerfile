FROM phplist/postfix:latest
COPY main.cf /etc/postfix/
ARG SERVER
ARG API_USER
ARG API_KEY
RUN echo $SERVER $API_USER:$API_KEY  >> /etc/postfix/sasl_passwd
RUN postmap /etc/postfix/sasl_passwd
RUN rm /etc/postfix/sasl_passwd
RUN chmod 600 /etc/postfix/sasl_passwd.db
