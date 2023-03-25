## Instalar o Docker no Ubuntu 20.04

Para instalar o Docker no Ubuntu 20.04, precisamos adicionar o repositório oficial do Docker ao nosso sistema e instalar o pacote docker-ce. Para isso, execute os seguintes comandos no terminal:

```bash
sudo apt update
sudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
sudo apt update
sudo apt install docker-ce
```