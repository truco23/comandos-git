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

##Tags
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



git blame                           = mostra quem realizou alterações no projeto
git ls-files                        = mostra os arquivos que o git está monitorando
*************************************

git branch                          = cria uma nova branch
git branch -b checkout nome_branch  = cria um nova branch e seleciona
git push -u origin nome_branch      = cria uma nova branch porém ao realizar pull não será necessário especificar o nome da nova branch
git branch -r                       = permite visualizar as branch remota
git checkout -t origin/design       = copiando a branch remota para local
git branch -a                       = lista as branch remotas e locais
git push -d origin design           = remove a branch remota
git fetch origin                    = verificar se foram criadas novas branch no repositório remoto
