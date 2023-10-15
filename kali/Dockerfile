ARG KALI_VERSION

FROM kalilinux/kali-rolling:${KALI_VERSION}

RUN apt -y update && apt -y upgrade && apt -y autoremove && apt clean

RUN apt -y install \
    pciutils \ 
    kmod

RUN apt -y install metasploit-framework

# Set working directory to /root
WORKDIR /root

# Open shell
CMD ["/bin/bash"]