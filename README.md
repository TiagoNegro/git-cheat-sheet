# GIT CHEAT SHEET

## Setup
git init                       # Inicialização de um repositório Git

git config --global user.name "Seu nome"

git config --global user.email "seu@email.com"

git config --lit               # Lista as configurações  

## Status e Log
git status                     # Verifica o status do repositório
git log                        # Exibe o histórico de commits do repositório
git log --oneline              # Exibe o histórico de commits resumido

## Adicionando e Gerar commit
git add <arquivo>              # Adiciona o arquivo para o staging
git add .                      # Adiciona tudo para o staging
git commit -m "mensagem"       # Commit com mensagem

## Branch
git branch                     # Lista todas as branches
git branch <nome>              # Cria nova branch
git checkout <nome>            # Troca para branch
git checkout -b <nome>         # Cria e troca para branch
git merge <branch>             # Mescla a branch atual com a especificada
git branch -d <nome>           # Delete a branch especificada

## Repositório remoto
git remote add origin <url>    # Adiciona repositório remoto
git push -u origin main        # Envia branch para repositório remoto
git push                       # Envia commits
git pull                       # Puxa alterações do repositório
git clone <url>                # Clona repositório

## Reversões
git restore                    # Desfaz as alterações no arquivo
git reset HEAD <arquivo>       # Remove o arquivo do staging
git reset --hard HEAD          # Desfaz tudo para o último commit
git revert <hash>              # Cria novo commit desfazendo o commit antigo

## Comparações
git diff                       # Mostra diferenças não commitadas
git diff --staged              # Mostra diferenças que vão ser commitadas
