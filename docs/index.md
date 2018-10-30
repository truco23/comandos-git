# Comandos Git


## Iniciando projeto
* Inicia um repositório utilizando o git
```
git init
```

## Configurações
* Adiciona um nome usuário
```
git config user.name "<nome usuário>"
```

* Adiciona um endereço de e-mail
```
git config user.email "<seu email>"
```

## Visualizando alterações
* Lista todos os arquivos que sofreram alguma alteração
```
git status
```

* Lista todos os arquivos que sofreram alguma alteração e o que foi alterado
```
git diff
```

* Mostra o que foi alterado no arquivo
```
git diff <nome arquivo>
```

## Preparando arquivos para o commit
* Adiciona um arquivo a sua staged área pronto para ser realizado um commit
```
git add <nome arquivo>
```

* Adiciona todos arquivos a sua staged área pronto para ser realizado um commit
```
git add -A
```


## Realizando commits
* Realiza um commit com uma mensagem de descrição
```
git commit -m "<mensagem de descrição>"
```

* Adiciona todos os arquivos alterados e uma mensagem de descrição
```
git commit -am <mensagem de descrição>
```

## Exibindo log
* Exibe log de commits e quais arquivos foram alterados
```
git whatchanged
git whatchanged -p
```

* Mostra todos os commits realizados 
```
git log
```

* Mostra todos os commits realizados de forma resumida de todas as branchs e um gráfico com histórico das alterações
```
git log --online --decorate --all --graph
```

## Repositório remoto
* Exibe as urls dos seus repositórios remotos
```
git remote
```

* Exibe a url e nome dos seus repositórios remotos
```
git remote -v
```

* Adiciona um repositório ao seu projeto local
```
git remote add <nome repositório> <url do repositório>
```

* Remonea repositório
```
git remote rename <nome antigo> <novo nome>
```

* Remove repositório
```
git remote remove <nome repositório>
```


## Enviando alterações
* Envia as alteraçõs locais para o repositório remoto
```
git push origin <nome branch>
```

## Tags
* Exibe todas as tags
```
git tag
```

* Exibe informações sobre a tag
```
git show <nome tag>
```

* Cria uma nova tag e adiciona uma mensagem de descrição
```
git tag -a <versao> -m "<comentario>"
```

* Envia a tag local para o repositório remoto
```
git push origin <nome-tag>
```

* Envia todas tag local para o repositório remoto
```
git push origin --tags
```

* Deleta tag do repositório remoto
```
git push --delete origin <nome tag>
```

* Deleta tag do repositório local
```
git tag -d <nome tag>
```

## Branchs
* Cria uma nova branch
```
git branch <nome branch>
```

* Cria uma nova branch e já muda para a nova branch
```
git branch -b checkout <nome branch>
```

* Envia a branch para o respositório remoto, sem a necessidade de especificar o nome da nova branch em um próximo push devido ao parâmetro -u
```
git push -u origin <nome branch>
```

* Visualizando as branch remotas
```
git branch -r
```

* Copiando a branch remota para local
```
git checkout -t origin/<nome branch>
```

* Listando as branch remotas e locais
```
git branch -a
```

* Removendo a branch remota
```
git push origin -d <nome branch>
```

* Removendo a branch local
```
git branch -d <nome branch>
```


git blame                           = mostra quem realizou alterações no projeto
git ls-files                        = mostra os arquivos que o git está monitorando
*************************************
