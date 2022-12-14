### Instalação de Ambiente Local!

Para usar a estrutura Angular, você deve estar familiarizado com o seguinte:

*  JavaScript (TypeScript)
*  HTML
*  CSS

Conhecimento de
TypeScript
é útil, mas não obrigatório.

Para instalar o Angular em seu sistema local, você precisa do seguinte:

*  Node: Angular requer um
LTS ativo ou LTS de manutenção
versão do Node.js.

*  Gerenciado de Pacotes: Os aplicativos Angular, Angular CLI e Angular dependem
pacotes npm
para muitos recursos e funções. Para baixar e instalar pacotes npm, você precisa de um gerenciador de pacotes npm. Este guia usa o
cliente npm
interface de linha de comando, que é instalada Node.jspor padrão. Para verificar se você tem o cliente npm instalado, execute npm -vem uma janela de terminal.

### Instale o Angular CLI

Você usa a CLI Angular para criar projetos, gerar código de aplicativo e biblioteca e executar uma variedade de tarefas de desenvolvimento contínuo, como teste, agrupamento e implantação.

```
  npm i -g @angular/cli
```

### Obs:

Em computadores cliente Windows, a execução de scripts do PowerShell é desabilitada por padrão. Para permitir a execução de scripts do PowerShell, necessários para binários globais npm, você deve definir o seguinte
política de execução:

```
  Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
```
Leia atentamente a mensagem exibida após a execução do comando e siga as instruções. Certifique-se de entender as implicações de definir uma política de execução

Apartir desse ponto vc ja vai estar com Angular/CLI instalado Globalmente no seu PC.
