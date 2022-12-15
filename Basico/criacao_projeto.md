### Criacao de Projeto

Apos feito a instalação do Angular/CLI via Gerenciador de Pacotes,
vamos testar ver se esta sendo identificado pelo terminal apenas digitando
ng --help se o retorno for esse: 

```
  Commands:
  ng add <collection>            Adds support for an external library to your project.
  ng analytics                   Configures the gathering of Angular CLI usage metrics.
  ng build [project]             Compiles an Angular application or library into an output directory named dist/ at
                                 the given output path.                                                  [aliases: b]
  ng cache                       Configure persistent disk cache and retrieve cache statistics.
  ng completion                  Set up Angular CLI autocompletion for your terminal.
  ng config [json-path] [value]  Retrieves or sets Angular configuration values in the angular.json file for the     
                                 workspace.
  ng deploy [project]            Invokes the deploy builder for a specified project or for the default project in the
                                 workspace.
  ng doc <keyword>               Opens the official Angular documentation (angular.io) in a browser, and searches for
                                 a given keyword.                                                        [aliases: d]
  ng e2e [project]               Builds and serves an Angular application, then runs end-to-end tests.   [aliases: e]
  ng extract-i18n [project]      Extracts i18n messages from source code.
  ng generate                    Generates and/or modifies files based on a schematic.                   [aliases: g]
  ng lint [project]              Runs linting tools on Angular application code in a given project folder.
  ng new [name]                  Creates a new Angular workspace.                                        [aliases: n]
  ng run <target>                Runs an Architect target with an optional custom builder configuration defined in   
                                 your project.
  ng serve [project]             Builds and serves your application, rebuilding on file changes.         [aliases: s]
  ng test [project]              Runs unit tests in a project.                                           [aliases: t]
  ng update [packages..]         Updates your workspace and its dependencies. See https://update.angular.io/.        
  ng version
```

com isso confirmamos o Angular e seguimos para a criação.
Escolha uma pasta(diretorio) no seu PC abra com VSCode ou Terminal e digite o seguinte comando:

```
  ng new nome_do_projeto
```

Aqui sera dado start no processo de geração do projeto perguntando se deseja enviar dados (S/N)

Selecione o modelo de stylus entre CSS, SCSS, LESS, ETC...

e aqui selecione que ira usar o Angular Routing (Sim isso aqui mais pra frente sera util).

Pronto so aguardar finalizar!

entre no projeto e execute o comando de launcher

```
  ng serve
```

Agora so acessar no browser http://localhost:4200