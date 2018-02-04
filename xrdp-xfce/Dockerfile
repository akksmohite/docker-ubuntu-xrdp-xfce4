FROM akshaym6/docker-ubuntu-xrdp:16.04

MAINTAINER Akshay Mohite <akksmohite@gmail.com>

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update -y && \
    #do not install recommnded packages
    #apt-get install -y  xfce4 --no-install-recommends  \
    apt-get install -y xfce4 xfce4-terminal gnome-icon-theme-full tango-icon-theme && \
    apt-get autoclean && apt-get autoremove && \
    rm -rf /var/lib/apt/lists/* && \
    echo "xfce4-session" > /home/xrdpuser/.xsession
