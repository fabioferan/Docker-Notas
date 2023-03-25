# Como instalar

## Como instalar o Docker no Windows

Existem diferentes maneiras de instalar o Docker no Windows, dependendo da sua versão do sistema operacional e dos requisitos de hardware. Você pode usar o Docker Desktop for Windows, que é um aplicativo que permite executar contêineres Linux e Windows com o WSL 2 ou o Hyper-V como backend. Você também pode usar o Docker Engine for Windows, que é um serviço que permite executar contêineres Windows com o Hyper-V como backend.

Para instalar o Docker Desktop for Windows, você precisa ter o Windows 10 ou 11 64-bit: Home ou Pro 21H1 (build 19043) ou superior, ou Enterprise ou Education 20H2 (build 19042) ou superior. Você também precisa habilitar o recurso WSL 2 no Windows e baixar e instalar o pacote de atualização do kernel Linux. Depois disso, você pode baixar o instalador do Docker Desktop for Windows no site do Docker e executá-lo seguindo as instruções na tela.

Para instalar o Docker no Windows, você pode seguir os seguintes passos:
1. Navegue até a página https://docs.docker.com/docker-for-windows/install/ e clique em Docker Desktop for Windows.
2. Inicie a instalação clicando duas vezes no Docker Desktop Installer.exe e em seguida, sim para para permitir que o instalador faça alterações em seu sistema.
3. Depois de instalado, inicie o Docker Desktop no menu Iniciar do Windows e selecione o ícone do Docker no menu ícones ocultos da barra de tarefas.
Verifique se "Usar o mecanismo baseado em WSL 2" está marcado em Configurações > Gerais.

Para instalar o Docker Engine for Windows, você precisa ter o Windows Server 2016 ou superior. Você pode baixar o instalador do Docker Engine for Windows no site do Docker e executá-lo usando um script PowerShell. Você também pode configurar o Docker Engine for Windows usando um arquivo de configuração em 'C:\ProgramData\Docker\config\daemon.json’.

## Como instalar o Docker no Linux

Existem várias formas de instalar o Docker no Linux, dependendo da sua distribuição e preferência. Uma forma simples é usar o snap, que é um sistema de gerenciamento de pacotes universal para Linux. Para isso, você precisa ter o snap instalado no seu sistema. Ele vem pré-instalado com a maioria das distribuições Linux, mas se não for encontrado, instale-o manualmente com o comando apropriado para o seu sistema operacional.

Depois de ter o snap instalado, você pode instalar o Docker com o seguinte comando:

```bash
sudo snap install docker
```

Outra forma é usar o repositório oficial do Docker, que permite instalar e atualizar o Docker com o apt. Para isso, você precisa adicionar a chave GPG e o repositório do Docker ao seu sistema, seguindo os passos descritos no site oficial do Docker.

```bash
sudo apt update
sudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
```

Depois de configurar o repositório, você pode instalar o Docker com o seguinte comando:

```bash
sudo apt update
sudo apt install docker-ce docker-ce-cli containerd.io
```

Há também outras formas de instalar o Docker no Linux, como usar um script bash, baixar um pacote binário ou usar um script de conveniência. Cada uma dessas formas tem suas vantagens e desvantagens, dependendo do seu caso de uso e necessidade.