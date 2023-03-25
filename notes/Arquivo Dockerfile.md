# Arquivo Dockerfile

Para escrever um Dockerfile, você precisa criar um arquivo sem extensão chamado “Dockerfile” com o editor de sua preferência. Esse arquivo deve conter instruções para criar uma imagem Docker. Essas instruções devem seguir um formato específico, incluir comandos como `FROM` para especificar a imagem base, são executadas em ordem e incluem a instalação de pacotes, criação de diretórios e definição de variáveis de ambiente entre outras coisas. É como uma receita de bolo que o Docker segue para construir a imagem.

Vamos criar um Dockerfile simples que instala o nginx (um servidor web) na imagem base do Ubuntu 20.04. Para isso, crie um arquivo chamado Dockerfile com o seguinte conteúdo:

```Dockerfile
# Imagem base
FROM ubuntu:20.04

# Atualizar os pacotes e instalar o nginx
RUN apt-get update && apt-get install -y nginx

# Expor a porta 80 do contêiner
EXPOSE 80

# Iniciar o serviço do nginx ao executar o contêiner
CMD ["nginx", "-g", "daemon off;"]
```

Depois de escrever o Dockerfile, você pode usar o comando `docker build` para construir a imagem a partir dele. A partir dessa imagem, você pode criar um container.

Alguns dos comandos mais úteis no Dockerfile incluem:

- `FROM`: especifica a imagem base a partir da qual você está construindo.
- `RUN`: executa um comando e cria uma nova camada na imagem. Por exemplo, é comum usar o comando `RUN` para instalar pacotes de software.
- `COPY`: copia arquivos e diretórios do seu sistema de arquivos local para a imagem.
- `ADD`: semelhante ao comando `COPY`, mas também pode ser usado para adicionar arquivos remotos e descompactar arquivos compactados.
- `CMD`: especifica o comando padrão a ser executado quando o contêiner é iniciado a partir da imagem.
- `EXPOSE`: informa ao Docker que o contêiner escutará em portas específicas em tempo de execução.

Esses são apenas alguns exemplos dos comandos disponíveis no Dockerfile. Você pode encontrar uma lista completa dos comandos na [documentação do Docker](https://docs.docker.com/engine/reference/builder/).