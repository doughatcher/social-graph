FROM mcr.microsoft.com/devcontainers/base:jammy

RUN sudo apt update && sudo apt install curl -y

RUN curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.0/install.sh | bash \
        && . $NVM_DIR/nvm.sh \
        && nvm install $NODE_VERSION \
        && nvm alias default $NODE_VERSION \
        && nvm use default

