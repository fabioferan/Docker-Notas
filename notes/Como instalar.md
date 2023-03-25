## Como instalar o Docker no Ubuntu 20.04

Para instalar o Docker no Ubuntu 20.04, precisamos adicionar o repositório oficial do Docker ao nosso sistema e instalar o pacote docker-ce. Para isso, execute os seguintes comandos no terminal:

```bash
sudo apt update
sudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
sudo apt update
sudo apt install docker-ce
```

## Como instalar o Docker no Windows

Existem diferentes maneiras de instalar o Docker no Windows, dependendo da sua versão do sistema operacional e dos requisitos de hardware. Você pode usar o Docker Desktop for Windows, que é um aplicativo que permite executar contêineres Linux e Windows com o WSL 2 ou o Hyper-V como backend. Você também pode usar o Docker Engine for Windows, que é um serviço que permite executar contêineres Windows com o Hyper-V como backend.

Para instalar o Docker Desktop for Windows, você precisa ter o Windows 10 ou 11 64-bit: Home ou Pro 21H1 (build 19043) ou superior, ou Enterprise ou Education 20H2 (build 19042) ou superior. Você também precisa habilitar o recurso WSL 2 no Windows e baixar e instalar o pacote de atualização do kernel Linux. Depois disso, você pode baixar o instalador do Docker Desktop for Windows no site do Docker e executá-lo seguindo as instruções na tela.

Para instalar o Docker no Windows, você pode seguir os seguintes passos:
1. Navegue até a página https://docs.docker.com/docker-for-windows/install/ e clique em Docker Desktop for Windows.
2. Inicie a instalação clicando duas vezes no Docker Desktop Installer.exe e em seguida, sim para para permitir que o instalador faça alterações em seu sistema.
3. Depois de instalado, inicie o Docker Desktop no menu Iniciar do Windows e selecione o ícone do Docker no menu ícones ocultos da barra de tarefas.
Verifique se "Usar o mecanismo baseado em WSL 2" está marcado em Configurações > Gerais.

Para instalar o Docker Engine for Windows, você precisa ter o Windows Server 2016 ou superior. Você pode baixar o instalador do Docker Engine for Windows no site do Docker e executá-lo usando um script PowerShell. Você também pode configurar o Docker Engine for Windows usando um arquivo de configuração em 'C:\ProgramData\Docker\config\daemon.json’.