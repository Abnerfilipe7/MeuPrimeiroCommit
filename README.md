# MeuPrimeiroCommit
## Configurar seu nome e e-mail

git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"

## Verificar a configuração atual
git config --list

## Criar um Novo Repositório
Inicializar um novo repositório
git init

Clonar um repositório existente
git clone https://github.com/usuario/repositorio.git

## Trabalhar com Arquivos
Ver o estado dos arquivos
git status

Adicionar arquivos à área de preparação (staging)
git add arquivo.txt
git add .   # Adiciona todos os arquivos modificados

Remover arquivos da área de preparação
git reset arquivo.txt

Remover arquivos do repositório
git rm arquivo.txt

## Confirmar Mudanças
Realizar um commit dos arquivos preparados
git commit -m "Mensagem do commit"

Modificar a mensagem do último commit (sem mudar o conteúdo)
git commit --amend

## Trabalhar com Branches
Listar branches
git branch

Criar um novo branch
git branch nome-branch

Criar e mudar para um novo branch
git checkout -b nome-branch

Fazer merge de um branch na branch atual
git merge nome-branch

Excluir um branch
git branch -d nome-branch

## Sincronização com o GitHub
Adicionar um remoto
git remote add origin https://github.com/usuario/repositorio.git

Verificar os remotos configurados
git remote -v

Enviar mudanças para o GitHub
git push origin nome-branch

Atualizar seu repositório local com mudanças do repositório remoto
git pull origin nome-branch

Obter informações sobre branches remotos
git fetch

## Histórico e Reversões
Ver o histórico de commits
git log

Ver o histórico de commits em uma linha
git log --oneline

Desfazer o último commit (sem eliminar as mudanças)
git reset --soft HEAD~1

Desfazer o último commit (e eliminar as mudanças)
git reset --hard HEAD~1