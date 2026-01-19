FROM node:latest

RUN apt-get update
RUN apt-get install -y git sudo

RUN useradd -ms /bin/bash developer
RUN usermod -aG sudo developer
RUN echo 'developer ALL=(ALL) NOPASSWD:ALL' > /etc/sudoers.d/developer
RUN chmod 0440 /etc/sudoers.d/developer

USER developer

RUN wget -qO- https://claude.ai/install.sh | bash
# for some reason this line will throw an error during build, so moved to postCreateCommand
# RUN claude mcp add myop https://mcp.myop.dev/mcp --transport http --scope user
RUN sudo npm install -g @myop/cli