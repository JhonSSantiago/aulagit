

### **Comandos git e github** :man_technologist:

##### Para instalar o Git use:

````bash
	$ sudo apt-get install git
````

##### Para Iniciar um repository:

````bash
	$ git init
````

##### verificar modificações nos arquivos:

````bash
	$ git status
````

##### Para adicionar arquivos a serem monitorados use:

````bash
	$ git add <nome_do_arquivo> ou * ou .
````

##### Remove um arquivo específico do monitoramento:

````bash
	$ git rm --cached <nome_do_arquivo>
````

##### Remove todos os arquivos do monitoramento:

````bash
	$ git rm --cached . -r
````

##### Para criar um registro do project use:

````bash
	$ git commit -m "comentario"
````

##### Enviando arquivos para para seu repositorio no GitHub

##### Para informar qual o respositório remoto será usado, use o comando:

````bash
	$ git remote add origin <link_do_repositório>
````

##### Para enviar os arquivos para o meu repositório remoto utilize o comando:

````bash
	$ git push -u origin <ramo>
````

##### Obtendo um Remote Repository use o comando:

````bash
	$ git clone <link_do_repositório>
````

#### Exibe o log de atividades
````bash
	$ git log
````

#### Retorna a um ponto específico de commit
````bash
	$ git checkout <numero_do_commit>
````

#### Retorna ao último commit realizado
````bash
	$ git checkcout <ramo>
````

#### Retorna a ramificações atual
````bash
	$ git branch
````

#### Cria uma nova ramificação
````bash
	$ git checkout -b <nome_da_ramificação_a_ser_criada>
````

#### Lista as ramificações
````bash
	$ git log --oneline
````

#### Para Fundir ramos
````bash
	$ git merge <ramo_para_fundir>
````

#### Mostra ramificação em grafico
````bash
	$ git log (-- oneline) --graph --all
````

#### Resolvendo conflitos no GitHub:

##### Esse comando mostra o arquivo e onde esta o conflito:

````bash
	$ git pull origin <ramo>
````


**-->** *Jhonatan Santiago*
