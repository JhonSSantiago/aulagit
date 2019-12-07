#Aula sobre Git
> Data: 29/11/2019

Iniciando com o Git

Para instalr o Git use:

````bash
	$ sudo apt-get install git
````

Para adicionar arquivos a serem monitorados use:

````bash
	$ git add
````

Para criar um registro do project use:

````bash
	$ git commit -m "comentario"
````
Enviando arquivos para para seu repositorio no GitHub

Abra o Github, faça login com a sua conta e clique em New repository.
Em seguida, basta colocar o nome e descrição do repositório que você está criando e clicar em Create repository.
Depois de criado, copie o link que esta disponivel logo abaixo do nome do repositorio.

Agora executar esse comando no terminal:

````bash
git remote add origin (link que voce copiou).
````
exemplo:

````bash
git remote add origin https://github.com/JhonSSantiago/aulagit.git
````

Basicamente o que estamos dizendo nessa linha de comando é:
"Git, esse meu repositório local se conectará com um remoto, o caminho dele(origin) é https://github.com/JhonSSantiago/aulagit.git Estabeleça essa comunicação pra mim".

Para enviar os arquivos para o meu repositório remoto utilize o comando:

````bash
git push -u origin master
````

--> Jhonatan da S. Santiago
