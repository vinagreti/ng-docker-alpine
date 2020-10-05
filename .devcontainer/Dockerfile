ARG VARIANT="12"

FROM mcr.microsoft.com/vscode/devcontainers/javascript-node:0-${VARIANT}

RUN echo "PS1='${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\[\033[01;34m\]\W\[\033[00m\]\$ '" > /home/node/.bashrc

RUN npm i

RUN export CHROME_BIN="/workspaces/ng-docker-alpine/node_modules/puppeteer/.local-chromium/linux-800071/chrome-linux"
