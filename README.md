# Imagem no Docker com Multistage Building
Na primeira etapa do Dockerfile, é feito o build do executável, tendo como imagem base o golang.<br />
Na segunda etapa, a partir de uma imagem leve (scratch) esse executável é rodado, tendo como resultado final o print da mensagem no terminal.

## Como utilizar
1) Build da imagem:<br />
Abra o terminal na pasta do projeto e rode:<br />
`docker build -t [nome da imagem] .`<br />

2) Run do container:<br />
Depois de criar a imagem rode o seguinte comando:<br />
`docker run -it --rm [nome da imagem]`<br />

**Link dessa imagem no meu DockerHub:** <br />
https://hub.docker.com/layers/anaanderi/fullcycle/latest/images/sha256:69d51d55f968b202fa7a0cb2a06d5f5c32c5b6e4a0289050e776a29c24f9d01e
