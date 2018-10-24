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

## Repositório local
* Exibe os repositórios do seu projeto
```
git remote
```

* Adiciona um repositório ao seu projeto local
```
git remote add url_repositorio
```

* Envia as alteraçõs locais para o repositório remoto
```
git push origin <nome branch>
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


***************************************

git tag                             = exibe todas as tags
git show <nome-tag>                 = exibe uma tag expecífica
git tag -a <versao> -m "<comentario>" = cria uma tag nome a versão e um comentário
git push origin <nome-tag>          = envia a tag para ambiente remoto