# Comandos úteis para desenvolvedores

<br
/>

## mkdir nome-do-diretorio

  <h4
>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Obs.: Nome do diretorio <strong>não pode ter espaço</strong> senão é gerado 2 diretórios, mais pode usar <strong>camelCase</strong> ou <strong>snack-case</strong>
</h4>

> <p
> >

    mkdir nome-do-diretorio

  </p>

> O comando mkdir gera diretório.

<br
/>

## lsof -i tcp:27017

<h4
>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Obs.: Utilizei quando, a porta do docker local, bloqueava subir o docker-compose. [tcp:27017] - este comando esta referenciando a porta que o deocker estava utilizando </h4>

> <p
> >

    lsof -i tcp:27017

  </p>

> O comando lsof (listar arquivos abertos) retorna os processos do usuário que estão usando ativamente um sistema de arquivos . Às vezes, é útil determinar por que um sistema de arquivos permanece em uso e não pode ser desmontado.

<br
/>

## docker ps -a

> <p
> >

    docker ps -a

 </p>

> O comando docker ps -a é para verificar os containers existentes na máquina -a é para verificar inclusive os inativos

<br
/>

## docker stop $(docker ps -a -q)

> <p
> >

    docker stop $(docker ps -a -q)

 </p>

> O comando docker stop $(docker ps -a -q) vai parar todos os containers da maquina (Full Completo), inclusive os que tiverem ocultos.

<br
/>

## docker rm $(docker ps -a -q)

> <p
> >

    docker rm $(docker ps -a -q)

 </p>

> O comando docker rm $(docker ps -a -q) vai remover todos os containers da maquina (Full Completo), inclusive os que tiverem ocultos. Porem as imagens que o container baixou na máquina ele não remove.

<br
/>

## docker volume prune

> <p
> >

    docker volume prune

 </p>

> O comando docker volume prune vai remover todos os volumes da maquina (Full Completo).

<br
/>

## docker rm -v container_name

> <p
> >

    docker rm -v container_name

 </p>

> O comando docker rm -v container_name vai remover 1 ou mais container por vez só acrescentar o nome do container o -v vai remover todos os volumes não nomeados.

<br
/>

## docker container inspect [CONTAINER_ID ou NAME]

> <p
> >

    docker container inspect [CONTAINER_ID ou NAME] 

 </p>

> O comando docker container inspect serve para fazer a inspeção completa de como o container foi criado, ele funciona tanto com ID do container como o nome do container

<br
/>

## docker-compose up -d

> <p
> >

    docker-compose up -d

 </p>

> O comando docker-compose up -d é para subir o docker-compose e o -d manter ativo na máquina.

<br
/>

## docker exec -it [nome-do-container ou o código] bash

> <p
> >

    docker exec -it [nome-do-container ou o código] bash

 </p>

 <h4
 >
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Obs.: Para sair so digitar exit e clicar no enter.</h4>

> O comando docker exec -it [nome-do-container ou o código] bash  este comando vai executar o docker-compose e te deixar dentro do container no terminal bash

<br
/>

## docker-compose down

> <p
> >

    docker-compose down

 </p>

> O comando docker-compose down é para baixar o docker-compose

<br
/>
