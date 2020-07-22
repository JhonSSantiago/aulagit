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

Obtendo um Remote Repository
Agora queremos pegar um Remote Repository e colocar o que está nele na sua máquina.

Eu sugiro que usemos o repositório github.com/PauloGoncalvesBH/treinamento-git no nosso treinamento.

Para fazer isso use o comando git clone https://github.com/PauloGoncalvesBH/treinamento-git.git

Mas, ao seguir este tutorial, você precisará enviar as alterações feitas no seu Dev Environment de volta ao Remote Repository, e o github não permite que uma pessoa faça isso no repositório de outra pessoa, por isso o melhor a fazer é criar um fork. Há um botão para fazer isso no canto superior direito desta página.

Agora que você já possui uma cópia do meu Remote Repository na sua conta do github por ter feito o fork, é hora de colocar isso em sua máquina.

Para isso usamos git clone https://github.com/{SEU USUÁRIO}/treinamento-git.git

Como você pode ver no diagrama abaixo, isso copia o Remote Repository em dois lugares, seu Working Directory e o Local Repository. Agora você vê como o git é um controle de versão distribuído. O Local Repository é uma cópia do Remote e age exatamente como ele. A única diferença é que você não o compartilha com ninguém.

O que o git clone também faz é criar uma nova pasta no local aonde você executou o comando. Deve haver uma pasta treinamento-git agora. Abra-a.

Adicionando coisas novas

Para ver o que está acontecendo no seu Working Directory execute git status, que informará em que branch você está, se o seu Local Repository é diferente do Remote e os arquivos tracked e untracked.

Você verá que Bob.txt não é rastreado (untracked) e o git status até lhe diz como mudar isso. Na figura abaixo, você pode ver o que acontece quando você segue a dica e executa git add Bob.txt: Você adicionou o arquivo à Staging Area, onde você coleta todas as alterações que deseja incluir no Repository.
--> Jhonatan da S. Santiago
