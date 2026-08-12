FROM mcr.microsoft.com/devcontainers/base:ubuntu

ENV DEBIAN_FRONTEND=noninteractive

# അത്യാവശ്യമായ പാക്കേജുകളും tmux ഉം ഇൻസ്റ്റാൾ ചെയ്യുന്നു
RUN apt-get update && apt-get install -y \
    curl \
    git \
    sudo \
    tmux \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

# ഡിഫോൾട്ടായി ഉബുണ്ടു യൂസർ ആയി വർക്ക് ചെയ്യാൻ
USER vscode
WORKDIR /home/vscode
