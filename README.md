# atalhos-git

//Git:

-Clone
git clone REPOSITORIO

-Nova branch
git checkout -b NOME_DA_BRANCH

-- Commit
git add .
git commit -m "MENSAGEM"
git push -u origin NOME_DA_BRANCH

-- Git Stash pilha de alterações antes e comitar
git stash // empilhar as alterações
git stash pop // voltar o ultimo item da pilha
git stash drop // Apaga da pilha

-- Configuração local
git config --local user.name "usuario"
git config --local user.email "email"

-- Reset
git reset --hard
git clean -fd
git gc

--cherry-pick
git log
pegar o hash da versão do log
criar uma nova branch
usar o comando git cherry-pick 'HASH do commit'

--Apagar branch local
git branch -D 'nome da branch'

--Sincronizar todos os repos locais com os do git
git fetch --all

--Rebase
ir para a master
dar um git pull
ir para sua branch
dar um git rebase master

--Git Amend (aproveitar o ultimo commit para correção: https://www.atlassian.com/br/git/tutorials/rewriting-history)
git commit --amend 

--Voltar um commit (usar git hub desktop)
git reset --hard HEAD^

-- Atualizar a tags locais
git fetch --all --tags 

-- Salvar as credenciais globais
git config --global credential.helper store

-- Corrigir 403 sem SSH
mudar url do arquivo .git/config = https://github-username@github.com/github-username/github-repository-name.git
ou via comando
git remote set-url origin https://github-username@github.com/github-username/github-repository-name.git

-- Git logs
https://devhints.io/git-log

-- visualizing-git
http://git-school.github.io/visualizing-git/
