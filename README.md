# comandos-GIT

## O que é GIT?

- Sistema de controle de versão distribuído
- Gratuito e Open Source
- Desenvolvido por Linus Torvalds para o desenvolvimento do Kernel Linux
- Download: https://git-scm.com/downloads

## Comandos básicos de GIT 

Inicializar um diretório existente como um repositório Git:
> git init

Copiar um diretório já existente:
> git clone [url do diretório]

Adicionar arquivos que serão versionados pelo Git (Stage):
> git add [nome do arquivo/arquivos]

> git add .

Commitar mudanças ou seja, gerar um identificador para as alterações realizadas nos arquivos do projeto:
> git commit

> git commit -m "Descrição/Comentário das modificações/alterações realizadas"

Renomear a mensagem do último commit feito:
> git commit --amend

Desfazendo o último commit:
> git revert HEAD

Enviar as alterações realizadas, e os arquivos adicionados para versionamento, para um repositório remoto:
> git push

> git push -u origin [nome da branch]

Capturar alterações que estejam salvas no repositório remoto, e não localmente.
> git pull

> git pull origin [nome da branch] 

Mostrar status das alterações feitas nos arquivos do repositório local:
> git status

Removendo arquivos do Stage, ou seja, se executou o git add e quer desfazer:
> git reset [nome do arquivo/arquivos]

Visualizar o histórico de commits:
> git log

Visualizar o histórico de um ou mais commits:
> git log -p [nome do arquivo/arquivos]

Visualizar o histórico de commits de um autor:
> git log --autor=[nome do autor]

Visualizar o histórico de commits por data:
> git log --after="MMM DD YYYY"

> git log --before="MMM DD YYYY"

Visualizar o histórico de commits baseado em uma mensagem:
> git log --grep "palavra que será utilizada para filtro"

Visualizar o histórico de commits de várias branchs:
> git log --all

- Navegar entre commits:
> git checkout [hash do commit para o qual se quer navegar]

Visualizar branchs de uma maneira mais legível:
> git log --all --decorate --oneline --graph

### Branchs

Listar as branchs do repositório local:
> git branch

Listar as branchs do repositório local e remoto:
> git branch -a

Criar uma nova branch:
> git branch [nome da branch]

Criar uma nova branch e ir direto para ela:
> git checkout -b [nome da branch]

Navegar entre branchs:
> git switch [nome da branch]

Excluir branchs locais, com -d ou -D:
- -d: só apaga a branch se você já tiver realizado o merge ou enviado as alterações para o repositório remoto.
- -D: ignora o estado da branch, forçando sua remoção.
> git branch -d [nome da branch]

> git branch -D [nome da branch]

Renomeando branchs:
> git branch -m [novo nome da branch]

> git branch -m nome_atual novo_nome



## Referências

Artigo web, escrito por Ana Paula de Andrade: [TREINAWEB](https://www.treinaweb.com.br/blog/primeiros-passos-com-o-git/)

Artigo web, escrito por Akira Hanashiro: [TREINAWEB](https://www.treinaweb.com.br/blog/comandos-do-git-que-voce-precisa-conhecer-parte-1)

Documentação oficial do GIT: [GIT - Documentation](https://git-scm.com/docs/git/pt_BR)
