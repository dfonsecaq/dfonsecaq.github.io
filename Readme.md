GitHub
https://github.com/
===================================================

--> udemy:criando páginas web com github pages
https://pages.github.com/
https://docs.github.com/pt/pages #help

New repositories
		dfonsecaq.github.io
Description
		Meu site pessoal
		Private
		
# Criando arquivos locais

mkdir MySite
	mkdir img
	touch Readme.md
	touch index.html
	
# Enviando arquivos para o GitHub
	
git init
git add .
  git config --global user.email "datral.system@gmail.com"
  git config --global user.name "dfonsecaq"
git remote add origin https://github.com/dfonsecaq/dfonsecaq.github.io.git
git commit -m "Arquivos iniciais"
git branch -M main
git push -u origin main		
git status

#Acessando o site
dfonsecaq.github.io


--< udemy:criando páginas web com github pages


--> 07/10/24 GitHub, primeira alteração
	http://github.com
	 datral.system@gmail.com
	  dfonsecaq , Dalécio Fonseca
	   pwd: ok! 
Git: versionamento de arquivos
GitHub: Platoforma de hospedagem de arquivos
Repositorios: pastas
 Main: linha cronologica principal
   Branch: ramificação da linha cronologica principal
 Commit: movimentação de arquivos, postar, salvar ...
 Merge: soma "Branch" 
 Remote: sistema no computador para trabalhar com github, 'faz o link'
 Push: colocar Commit da maquina no Remote, la no github
 Pull: contrario do Push, pega arquivos atualizados no GitHub para baixar na maquina
 
 Install: Git-2.46.2-64-bit
   Veio com terminais:
    Git bash
	Git cmd
    Git GUI: para criar ou executar repositorios na maquina
 Usando Git bash: #info Rafaela
    Git--version 
	usando o 'Git bash' criei o diretorio:
	 C:\Users\dalecio\Documents\Program\GitHub\Git_T01: "Repositorio local"
	 touch Readme.md # md: linguagem de marcação
	 Readme.md , tem todas as diretrizes deste comit
    Comandos no bash:
	 
Repositorios 'na maquina Dell T3500/oficina'
 C:\Users\dalecio\Documents\Program\GitHub\
  Git_T01 # T de teste, cd para o diretorio do repositorio
		git init # no bash, a GUI ja inicializa automatico, cria "master ou Main"
		  caso queira mudar de master para main use: git branch -M "main"
		git add Readme.md # adiciona arquivos para commit "area de stage(fase)"
		git status # mostra arquivos a serem comitados
		git commit -m "primeiro commit" # "titulo do commit"
		 Erro:Author identity unknown, Please tell me who you are. Run:
		  git config --global user.email "you@example.com"
		   git config --global user.email "datral.system.com"
          git config --global user.name "Your Name" dfonsecaq
		   git config --global user.name "dfonsecaq"
		  Omit --global to set the identity only in this repository.
Repositorios no 'GitHub'
  Entrar na conta do HitHub e executar 'New'
	Repository name: mesmo da maquina 'Git_T01' não aceitou 'Git_T01-first'	foi aceito  
	Description: 'Meu primerio repositorio da maquina T3500 /oficina'
	Apos comando 'create', aparece as informações:
		https://github.com/dfonsecaq/Git_T01-first.git
		 'ssh': git@github.com:dfonsecaq/Git_T01-first.git
		create a new repository on the command line
		echo "# Git_T01-first" >> README.md #terminal Git cmd
		git init
		git add README.md
		git commit -m "first commit"
		git branch -M main
		git remote add origin https://github.com/dfonsecaq/Git_T01-first.git
		git push -u origin main
		
		push an existing repository from the command line
		git remote add origin https://github.com/dfonsecaq/Git_T01-first.git
		git branch -M main
		git push -u origin main
	git remote add origin https://github.com/dfonsecaq/Git_T01-first.git #origin = nome do repositorio do GitHub
	git push -u origin master #não aceitou usuario e senha"remote: Support for password authentication was removed on August 13, 2021."
	
	PAT (Personal Access Token)
	Create Personal Access Token on GitHub #home, clicar na foto.
	From your GitHub account, go to Settings ? Developer Settings 
	? Personal Access Token ? Tokens (classic) ? Generate New Token
	(Give your password) ? Fillup the form ? click Generate token 
	? Copy the generated Token, it will be something like 
	ghp_sFhFsSHhTzMDreGRLjmks4Tzuzgthdvfsrta
	
	token for user until 90 days: The token will expire on Sun, Jan 5 2025
	  [x] todas as opções
	  gerado: ok!
	Agora 'git push -u origin master'
	  usuario e token funcionou!
	  
	$ git push -u origin master
	Enumerating objects: 3, done.
	Counting objects: 100% (3/3), done.
	Delta compression using up to 4 threads
	Compressing objects: 100% (2/2), done.
	Writing objects: 100% (3/3), 249 bytes | 249.00 KiB/s, done.
	Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
	To https://github.com/dfonsecaq/Git_T01-first.git
	 * [new branch]      master -> master
	branch 'master' set up to track 'origin/master'.
--<07/10/24 GitHub, primeira alteração