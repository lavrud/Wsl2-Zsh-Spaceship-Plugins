![link](https://assets.ubuntu.com/v1/ad89548e-ubuntu-on-wsl.png)

Este tutorial trata-se de como configurar o Wsl2 (subsistema Ubuntu 18.04 LTS) no Windows 10/11, assim como instalar packages, themes, plugins e fonts.

## WSL2

Acesse este link para _[Instalar o WSL](https://docs.microsoft.com/pt-br/windows/wsl/install)_, análise os pré-requisitos <br> instale em sua máquina windows e siga o passo-a-passo para executar.

## ZSH

• Instalar Zsh: <code>sudo apt install zsh</code>  
• Definir Zsh como padrão: <code>chsh -s $(which zsh)</code>

## OH-MY-ZSH

• Instalar Curl+Git: <code>sudo apt install curl git -y</code>  
• Instalar Oh-My-Zsh: `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
