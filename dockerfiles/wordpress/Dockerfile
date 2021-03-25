FROM wordpress:latest

RUN \
    curl --location --output /usr/local/bin/mhsendmail https://github.com/mailhog/mhsendmail/releases/latest/download/mhsendmail_linux_amd64 \
    && chmod +x /usr/local/bin/mhsendmail \
    && echo 'sendmail_path="/usr/local/bin/mhsendmail --smtp-addr=mailhog:1025 --from=no-reply@example.com"' > /usr/local/etc/php/conf.d/mailhog.ini