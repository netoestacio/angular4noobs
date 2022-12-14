### Arquitetura do Framework!

### NgModules
A arquitetura de um aplicativo Angular depende de alguns conceitos básicos. Em síntese, os blocos de construção básicos da estrutura são componentes organizados em NgModules. 

Um NgModule declara um contexto de compilação para um conjunto de componentes dedicado a um domínio de aplicativo, um fluxo de trabalho ou um conjunto de recursos intimamente relacionados. 

Além disso, os NgModules coletam o código relacionado em conjuntos funcionais, desse modo, uma aplicação Angular é definida por um conjunto de NgModules. 

Todo aplicativo construído com esse framework terá um módulo raiz, chamado AppModule, que fornece o mecanismo de bootstrap para iniciar o aplicativo, em geral, um app normalmente terá muitos módulos funcionais.

Para os desenvolvedores, organizar o código em módulos funcionais diferentes auxilia no desenvolvimento e no design.

Além disso, possibilita o aproveitamento do carregamento lento, isto é, usa o carregamento de módulos sob demanda para minimizar a quantidade de código para ser carregado na inicialização.

### Components
Como citamos, um aplicativo Angular possui ao menos um componente, chamado raiz, com a função de conectar uma hierarquia de componentes com o modelo de objeto de documento de página (DOM). 

Cada um dos componentes estabelece uma classe que contém dados e lógica, e está associado a um modelo HTML que define uma visualização a ser exibida em um ambiente de destino.

O decorator @Component() identifica a classe imediatamente como um componente e oferece o modelo e os metadados específicos dele.

Esses metadados configuram, por exemplo, como o componente pode ser referenciado no HTML e quais os serviços devem ser utilizados.
```
  @Component({
  selector: ‘app-root’,
  templateUrl: ‘./app.component.html’,
  styleUrls: [‘./app.component.css’],
  providers: [ HeroService ]
  })
```
### Decorador de classe
Um decorador que aparece logo antes de uma definição de classe, que declara que a classe é do tipo fornecido e oferece metadados adequados ao tipo. Os seguintes decoradores podem declarar tipos de classe Angular:
```
  @Component()
  @Directive()
  @Pipe()
  @Injectable()
  @NgModule()
```

### Directives
São como marcadores no elemento DOM que comunicam ao Angular para incluir um comportamento específico. Existem três modelos de diretivas nesse framework: Diretivas estruturais, Diretivas de atributos e Componentes.

Diretivas estruturais: modificam o layout adicionando ou removendo elementos do DOM, por exemplo, NgIf e NgFor.

Diretivas de atributos: alteram a aparência ou o comportamento do elemento, componente ou outra diretiva, por exemplo, NgClass e NgStyle.

Componentes: são diretivas com um modelo.

### Interpolation
Nesse framework a interpolação é usada para exibir uma propriedade do componente no HTML.


Neste caso, sua sintaxe são chaves duplas e podemos exibir qualquer tipo de dados, por exemplo, números, datas, entre outros parâmetros.
```
    Componente
    export class AppComponent {
    propriedade = “Hello!!!”
    }

  Html
  <h1>{{propriedade}}</h1>
```
### Dependency Injection (DI)
Dependências são serviços ou objetos que uma classe precisa para desempenhar sua função. Nesse sentido, injeção de dependência, ou DI, é um padrão de design no qual uma classe solicita dependências de fontes externas em vez de criá-las.

Além disso, a injeção de dependência (DI) permite manter as classes de componentes enxutas e eficientes. O DI é conectado à estrutura e usado em todos os lugares para fornecer aos componentes os serviços.

Componentes consomem serviços, assim sendo, você pode injetar um serviço em um componente, dando acesso ao componente para essa classe de serviço.

Para isso, é utilizado o providedIn, uma propriedade do decorador @Injectable.
```
  @Injetable({
  providedIn: SomeModule
  })
```
### Angular CLI
Essa é uma ferramenta de interface de linha de comando utilizada por desenvolvedores para inicializar, desenvolver, estruturar e manter os aplicativos criados com esse framework.

É possível usar a ferramenta diretamente em um shell de comando (software independente que oferece comunicação direta) ou indiretamente através da interface do usuário interativa, por exemplo, o Angular Console.

Para exemplificar, os comandos a seguir demonstram como o uso de Angular CLI facilita o trabalho do desenvolvedor Angular. Veja alguns deles:

*  ng build: compila um aplicativo Angular em um diretório de saída.
*  ng serve: cria um servidor local HTTP para testar o aplicativo, reconstruindo as alterações do arquivo.
*  ng generate: gera ou modifica arquivos com base em um esquema.
*  ng test: executa testes de unidade em um determinado projeto.
*  ng e2e: constrói e fornece um aplicativo e executa testes de ponta a ponta.

### Angular SPAs
Esse é uma Single-Page Application, uma aplicação web que roda em uma única página, semelhante a um aplicativo desktop ou mobile. Pode ser chamada de página ajax.

Usar esse framework para fazer uma SPA é uma boa alternativa, pois possui sistemas de rotas e clientes HTTP para fazer requisições a recursos externos, por exemplo, uma API.