git init                            = inicia um repositório com o git
git config user.name "nome user"    = adiciona nome usuário
git config user.email "email user"  = adiciona email usuário
git blame                           = mostra quem realizou alterações no projeto
git ls-files                        = mostra os arquivos que o git está monitorando
git add                             = adiciona um arquivo novo à ser monitorado / arquivo alterado
# Comandos Git

* Iniciar um repositório utilizando o git
```
git init
```

* Adicionar arquivo e realizar commit juntamente com uma mensagem
```
git commit -am
```

git whatchanged/git whatchanged -p  = exibe log de commits e quais arquivos foram alterados
git remote                          = exibe os repositórios do seu projeto
git remote add url_repositorio      = adiciona um repositório ao seu projeto local


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