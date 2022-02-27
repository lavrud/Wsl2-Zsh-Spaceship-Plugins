![link](https://assets.ubuntu.com/v1/ad89548e-ubuntu-on-wsl.png)

Este tutorial trata-se de como configurar o Wsl2 (subsistema Ubuntu 18.04 LTS) no Windows 10/11, assim como instalar packages, themes, plugins e fonts.

## WSL2

Acesse este link para _[Instalar o WSL](https://docs.microsoft.com/pt-br/windows/wsl/install)_, análise os pré-requisitos <br> instale em sua máquina windows e siga o passo-a-passo para executar.

## ZSH

• Instale o Zsh: `sudo apt install zsh`<br>
• Defina o Zsh como padrão: `chsh -s $(which zsh)`

## OH-MY-ZSH - _[link](https://ohmyz.sh/)_

• Instale Curl+Git: `sudo apt install curl git -y`<br>
• Instale Oh-My-Zsh: `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`<br>
• Restart terminal (executando prompt de comando em modo administrador): `wsl --shutdown`<br>
_Obs: Depois de executar o comando acima, feche o terminal e reabra o terminal shell(linux)_

## FIRA CODE - _[link](https://github.com/tonsky/FiraCode)_

• Baixe informações de todos os pacotes de fontes configuradas: `sudo apt update`<br>
• Instale a fonte Fira Code: `sudo apt install fonts-firacode`<br>

## SPACESHIP - _[link](https://github.com/spaceship-prompt/spaceship-prompt)_

• Clone este repositório: `git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1`<br>
• Crie um Symlink(link simbólico) para o diretório custom/themes: `ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"`<br>
• Defina `ZSH_THEME="spaceship"` em seu `~/.zshrc`

## ZINIT Plugin - _[link](https://github.com/zdharma-continuum/zinit)_

• Instale Zinit: `sh -c "$(curl -fsSL https://git.io/zinit-install)"`<br>
• Abra o arquivo `~/.zshrc` novamente e abaixo da linha _### End of ZInit's installer chunk_ escreva:

`zinit light zdharma/fast-syntax-highlighting`<br>
`zinit light zsh-users/zsh-autosuggestions`<br>
`zinit light zsh-users/zsh-completions`
