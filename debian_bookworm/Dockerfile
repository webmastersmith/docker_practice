FROM debian:bookworm
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
RUN apt update && apt install git python3-pip ansible nano openssh-client -y
# RUN useradd -m ansible
# RUN mkdir -p /home/ansible/.ssh
# COPY id_rsa_shared /home/ansible/.ssh/id_rsa
# RUN chown -R user:user /home/user/.ssh
# RUN echo "Host remotehost\n\tStrictHostKeyChecking no\n" >> /home/user/.ssh/config
# USER user
# keep container from closing.
CMD ["/bin/bash"]
