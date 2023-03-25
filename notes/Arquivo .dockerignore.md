
# Arquivo .dockerignore

Um arquivo `.dockerignore` é um arquivo de texto que especifica quais arquivos e diretórios devem ser ignorados ao copiar arquivos do seu sistema de arquivos local para a imagem Docker durante a construção. Ele funciona de maneira semelhante a um arquivo `.gitignore` usado com o Git.

Para criar um arquivo `.dockerignore`, basta criar um arquivo de texto com o nome `.dockerignore` no mesmo diretório que o seu Dockerfile. Em seguida, você pode adicionar padrões de nome de arquivo e diretório para ignorar ao copiar arquivos do seu sistema de arquivos local para a imagem Docker durante a construção.

Por exemplo, para ignorar todos os arquivos `*.log` e o diretório `temp`, você pode criar um arquivo `.dockerignore` com o seguinte conteúdo:

```
*.log
temp/
```

Depois de criar o arquivo `.dockerignore`, ele será automaticamente usado pelo Docker durante a construção da imagem para ignorar os arquivos e diretórios especificados. Isso pode ajudar a reduzir o tamanho da imagem e também acelerar o tempo de construção.

Você pode encontrar mais informações sobre como usar o arquivo `.dockerignore` na [documentação do Docker](https://docs.docker.com/engine/reference/builder/#dockerignore-file).