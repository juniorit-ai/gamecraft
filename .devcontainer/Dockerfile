FROM haicam/juniorit-clang:v1.0.3

ARG JUNIORIT_DEV_VER=v1.0.4

ARG USERNAME=juniorit

USER root

COPY php.ini /usr/local/etc/php.ini
ENV LANG en_US.UTF-8
ENV LANGUAGE en_US:en
ENV LC_ALL en_US.UTF-8
ENV JUNIORIT_DEV_VER $JUNIORIT_DEV_VER
ENV PHP_INI_SCAN_DIR /usr/local/etc

WORKDIR /home/$USERNAME/workspace
USER $USERNAME

ENTRYPOINT /usr/local/bin/jdaemon