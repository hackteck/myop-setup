FROM node:latest

RUN apt-get update
RUN apt-get install -y git sudo

RUN useradd -ms /bin/bash developer
RUN usermod -aG sudo developer
RUN echo 'developer ALL=(ALL) NOPASSWD:ALL' > /etc/sudoers.d/developer
RUN chmod 0440 /etc/sudoers.d/developer

USER developer

RUN wget -qO- https://claude.ai/install.sh | bash