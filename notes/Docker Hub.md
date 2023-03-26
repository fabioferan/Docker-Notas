# Docker Hub

Para enviar sua imagem Docker para o Docker Hub, você precisa primeiro criar uma conta no Docker Hub e fazer login na linha de comando usando o comando `docker login`. Depois de fazer login, você pode usar o comando `docker push` para enviar sua imagem para o Docker Hub.

Antes de enviar a imagem, é importante que você marque a imagem com o nome do seu repositório no Docker Hub. Por exemplo, se seu nome de usuário no Docker Hub é `meu-usuario` e você deseja enviar a imagem `minha-imagem` para um repositório chamado `meu-repositorio`, você pode usar os seguintes comandos:

```Bash
docker tag minha-imagem meu-usuario/meu-repositorio:minha-imagem
docker push meu-usuario/meu-repositorio:minha-imagem
```

O primeiro comando marca a imagem `minha-imagem` com o nome do repositório no Docker Hub (`meu-usuario/meu-repositorio`) e a tag da imagem (`minha-imagem`). O segundo comando envia a imagem marcada para o Docker Hub.

Depois que a imagem for enviada com sucesso, ela estará disponível publicamente no Docker Hub e poderá ser baixada por qualquer pessoa usando o comando `docker pull`.