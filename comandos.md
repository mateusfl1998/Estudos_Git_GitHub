#### Fazer:
- Tentar fazer as alterações

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

- Merge
- [AngularJS] - HTML enhanced for web apps!
- [Ace Editor] - awesome web-based text editor
- [markdown-it] - Markdown parser done right. Fast and easy to extend.
- [Twitter Bootstrap] - great UI boilerplate for modern web apps
- [node.js] - evented I/O for the backend
- [Express] - fast node.js network app framework [@tjholowaychuk]
- [Gulp] - the streaming build system
- [Breakdance](https://breakdance.github.io/breakdance/) - HTML
to Markdown converter
- [jQuery] - duh

And of course Dillinger itself is open source with a [public repository][dill]
 on GitHub.

## [Curso de Git e GitHub - 2023] Aula 5.1: na prática - git commit, add, push e outros.


Dillinger requires [Node.js](https://nodejs.org/) v10+ to run.

Install the dependencies and devDependencies and start the server.

```sh
cd dillinger
npm i
node app
```

For production environments...

```sh
npm install --production
NODE_ENV=production node app
```

## Plugins

Dillinger is currently extended with the following plugins.
Instructions on how to use them in your own application are linked below.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |

## Development

Want to contribute? Great!

Dillinger uses Gulp + Webpack for fast developing.
Make a change in your file and instantaneously see your updates!

Open your favorite Terminal and run these commands.

First Tab:

```sh
node app
```

Second Tab:

```sh
gulp watch
```

(optional) Third:

```sh
karma test
```

#### Building for source

For production release:

```sh
gulp build --prod
```

Generating pre-built zip archives for distribution:

```sh
gulp build dist --prod
```

## Docker

Dillinger is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 8080, so change this within the
Dockerfile if necessary. When ready, simply use the Dockerfile to
build the image.

```sh
cd dillinger
docker build -t <youruser>/dillinger:${package.json.version} .
```

This will create the dillinger image and pull in the necessary dependencies.
Be sure to swap out `${package.json.version}` with the actual
version of Dillinger.

Once done, run the Docker image and map the port to whatever you wish on
your host. In this example, we simply map port 8000 of the host to
port 8080 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --restart=always --cap-add=SYS_ADMIN --name=dillinger <youruser>/dillinger:${package.json.version}
```

> Note: `--capt-add=SYS-ADMIN` is required for PDF rendering.

Verify the deployment by navigating to your server address in
your preferred browser.

```sh
127.0.0.1:8000
```

## License

MIT

**Free Software, Hell Yeah!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>