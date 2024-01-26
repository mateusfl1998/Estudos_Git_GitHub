Link do Curso: 

#### Fazer:
- Tentar fazer as alterações
- Ver boas práticas de programação

## [Curso de Git e GitHub - 2023] Aula 1: Versionamento de Código

O sistema de controle de versão de código serve para 2 ou mais pessoas irem trabalhando simultâneamente num código! 
- Registra o histórico de mudanças!
- Últil para enteder o que foi feito e quando foi feito!

#####  Plataformas de versionamento de código:
Visto:
> É instalada na máquina local, o Git Hub é apenas o armazenamento de código em núvem!

- Git
- Subversion (SVN) - Tortoise SVN
- 

#####  Plataformas hospedagem de códigos em nuvem:
- GitLab
- GitHub
- SourceForge
- 
**Outros pontos importantes da aula:**
**CLI:** COMAND LINE INTERFACE
**CD:** CHANGE DIRECTORY 

# [Curso de Git e GitHub - 2023] Aula 2: Monitoramento de estados e ambientes

**Como funciona:** Alterações realizadas no meu código (Eu salvo com CTRL P) >> Escolher o que eu quero comitar(STAGE) - ISSO É O GIT ADD. >> Dou o  Commit >> Tenho os históricos de commits

Histórico de alterações comitadas (commit story)

# [Curso de Git e GitHub - 2023] Aula 3: Principais comandos GIT

- git init (inicia o repositório)
- Git clone <nome_do_repositório>
- git branch <nome_da_branch> (cria uma nova branch)
- git push - envia as alterações]
- git log (visualizar histório de alterações)
- git stash
- git diff (verifica as diferenças dos códigos)
- git pull - puxa as alterações
- git merge 
- git branch (verifica as branches local)
- git branch -a (vê as branchs remotas)
- git add . (adiciona o arquivo ao controle de versão)
- git log (lista de commits que já foram feitas) 
- git log - -  pretty=oneline ()
- git checkout -b 'nova-feature' (nesse comando vc entra e cria a branch)
- git status
- git add coloca as informações no stage
- git branch -M 'novo nome' - (renomeia a branch atual)
- git remote add origin 'url do repositório' (informa o diretório que vamos conectar)
- git remote get-url origin
- git --set-upstream origin nome da branch

## [Curso de Git e GitHub - 2023] Aula 4: setup e configuração do ambiente de programação para GIT

> Instale as seguintes extensões no visual estudio code: Git Graph e o Git History

## [Curso de Git e GitHub - 2023] Aula 5: git commit

Dica 1 : adicione apenas as mudanças certas ao commit. 
Dica 2: evite fazer um único commit para todo o código escrito.

**Controlando o que vai ser ou não commitado:**
1 - git diff: visualizar as alterações
2 - git status: para ver as alterações vão ser comitadas
3 - git add: para adicionar as alterações ao commit.

Dica: escrever commit: git commit -m 'titulo' -m 'corpo do texto'
Seja mais direto possível no título. No corpo do texto descreva o motivo da mudança, informações extras, cuidados, alertas. O corpo do texto pode ser mais detalhado.

**Git ignore:** os arquivos que não devem ser comitados você precisa coloca-los aqui.env.(dotenv    )

### Fluxo do git commit:
 - salvar código
 - dar git add (adiciona ao stage)
 - git commit (comita localmente)
 - git push (joga para nuvem)



# [Curso de Git e GitHub - 2023] Aula 5.1: na prática - git commit, add, push e outros.

README.MD é a explicação do repositório. Data, como foi feito, como usar e etc!

Quando os arquivos da direita estão verdes significa que eles não estão sendo rastreados pelo git. Você tem que digitar 'git commit'   

A - Fica index add. Fala que o arquivo 
M - Diz que o arquivo foi modificado 

Dica: padrão para repositórios do git 'nome-sobrenome'

Branch 'MASTER' normalmente é uma branch que vai existir para longo prazo. 

Como eu escolho somente uma única modificação para ir para o commit: git restore --staged <nome do arquivo>

Primeira vez que vc digita o comando push você tem que digitar: git push -u origin main

Vc informa aqui qual a push que você quer subir



# [Curso de Git e GitHub - 2023] Aula 5.2: na prática - como analisar o histórico de commits

git blame

# [Curso de Git e GitHub - 2023] Aula 6: o que são branches?

Modelos de Controle de Versão:

Branches Únicas, Git Flow, GitHub Flow

Existem básicamente Branches de stats (que não mexe, branch de versões de software e branch de fetarures ( para criar um funcionalidade nova dentro do aplicativo e nao arriscar a estabilidade da branch principal))

```
Branchs são trilha de commits! Trilho/árvore

Pode ter propósitos destintos: para fazer testes
```

```
Branches "long-running": são branches que ficam vivas por longo tempo. "main"  e "develop"
```

```
Branches "shoted.lived": implementar funções ou corrigir bugs
```
### TIPOS DE BRANCH:

**Branch única:** normalmente usada quando somente uma pessoa está mexendo no código! Muito comum em projetos pessoais

Veja como funciona o GitHubFlow: https://prnt.sc/5IuPyoIpeP0O

Depois vc dá um merge de uma branch para outra.

**GitHub Flow:** modelo gitflow: https://prnt.sc/FpS3_mY0A8Lb

resumindo: existe alguns tipos de branch, as mais usadas são branch de features e branchs de fix. 

## [Curso de Git e GitHub - 2023] Aula 6.1: na prática - git push, pull requests & code reviews.

Você faz o pull request para pedir ao desenvolvedor no comando colocar a atualização da feature que vc fez na branch main

# [Curso de Git e GitHub - 2023] Aula 7: Pull Requests

Pull request: é pedir que seu código seja incluido no projeto!

**Pull requestes de branchs públicas e privadas!**

```
**Privadas**: cria branch "short-live" a partir da branch de desenvolvimento e depois faz pull request"

```
```
**Públicos**: você clona o repositório original (aqui vc não cria a branch, ou cria =D) e depois faz um pull request "
     
```

#### Code Review:
Aula de como funciona: https://prnt.sc/jFNza43Tlxkh

## [Curso de Git e GitHub - 2023] Aula 8: git merge & conflitos

**O que são conflitos:** Por exemplo você escreveu x na linha de código 10 de um arquivo, e eu também escrevi na linha 10 y.Ai na hora da gente integrar nossos códigos, nós temos um conflito 

_Comandos que podem gerar conflitos:_ merge,rebase, pull, stash, apply

**Como resolver**: 

- Escolher manter 1 ou a outra alteração
- Inserir as 2 alterações. Qual linha vai aparecer primeiro?
- Remover as 2 alterações
- Cancelar o Merge

Fluxo de solução: https://prnt.sc/63uZKmqxgRGf

Todo dia antes de codar, faça o pull do código

**DICA**: resolva os conflitos o mais rápido possível. Pois se não resolver, pode ir surgindo mais conflitos 

Fluxo de ações para solução de conflitos: https://prnt.sc/aaZ8icTpIT_J

# [Curso de Git e GitHub - 2023] Aula 8.1: na prática - resolvendo conflitos.

Essa aula foi mais de prática. 

Para apagar uma branch local  

**git branch -d 'nome da branch'**

Para apagar uma branch remota 

**git branch -d origin 'nome da branch'**

# git[Curso de Git e GitHub - 2023] Aula 9: git stash

para que fazer? git impedindo merge/ou publicação de alterações

Mais informações: https://prnt.sc/KbK7gCEQUeHE

git stash: guardar no stash (bolso)
git stash pop: recuperar do stash

# [Curso de Git e GitHub - 2023] Aula 9.1: na prática - git pull & atualização de repositório local.

Mantendo sua branch atualizada

Aula mais prática!

**Deletar a branch local:** git branch -d nome da branch

**Deletar a branch remota** git push -d origin nome da branch

# [Curso de Git e GitHub - 2023] Aula 10: git revert & git reset

git revert: comando para desfazer mudançase em um repositório 

ele cria um commit novo que inverte todas as alterações desejadas!

mapa ilustratório: https://prnt.sc/6uKF9ZEiaaik

a diferença do git revert para o git reset: é que o git reset desfaz as alterações do commit 

Cuidado ao utilizar o git reset, **é melhor utilizar o git revert**

# [Curso de Git e GitHub - 2023] Aula 10.1: na prática - desfazendo alterações com git revert.

Aula mais pratica, comandos utilizados:

git revert HEAD

> Note: `--capt-add=SYS-ADMIN` is required for PDF rendering.

Verify the deployment by navigating to your server address in
your preferred browser.
