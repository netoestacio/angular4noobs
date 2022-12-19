 ### Compoents

 Os componentes são o bloco de construção principal para aplicativos Angular. Cada componente consiste em:

*  Um modelo HTML que declara o que é renderizado na página
*  Uma classe TypeScript que define o comportamento
*  Um seletor CSS que define como o componente é usado em um modelo
*  Opcionalmente, estilos CSS aplicados ao mode

## Criando um Component

A melhor maneira de criar um componente é com o Angular CLI. Você também pode criar um componente manualmente.

Para criar um componente usando o Angular CLI:

*  Em uma janela de terminal, navegue até o diretório que contém seu aplicativo.
*  Execute o ng generate component <component-name>comando, onde <component-name>está o nome do seu novo componente.

Por padrão, esse comando cria o seguinte:

*  Um diretório com o nome do componente
*  Um arquivo componente,<component-name>.component.ts
*  Um arquivo de modelo,<component-name>.component.html
*  Um arquivo CSS,<component-name>.component.css
*  Um arquivo de especificação de teste,<component-name>.component.spec.ts

Onde <component-name>está o nome do seu componente.

## Criando um componente manualmente

Embora a CLI Angular seja a melhor maneira de criar um componente Angular, você também pode criar um componente manualmente. Esta seção descreve como criar o arquivo de componente principal dentro de um projeto Angular existente.

Para criar um novo componente manualmente:

*  Navegue até o diretório do projeto Angular.
*  Crie um novo arquivo, <component-name>.component.ts.
*  Na parte superior do arquivo, adicione a seguinte instrução de importação.
```
  import { Component } from '@angular/core';
```
*  Após a importinstrução, adicione um decorador.@Component
```
  @Component({
  })
```
*  Escolha um seletor de CSS para o componente.
```
  @Component({
   selector: 'app-component-overview',
  })
```
Para obter mais informações sobre como escolher um seletor, consulte Especificando o seletor de um componente .

*  Defina o modelo HTML que o componente usa para exibir informações. Na maioria dos casos, esse modelo é um arquivo HTML separado.
```
  @Component({
   selector: 'app-component-overview',
    templateUrl: './component-overview.component.html',
  })
```
Para obter mais informações sobre como definir o modelo de um componente, consulte Definindo o modelo de um componente .

*  Selecione os estilos para o modelo do componente. Na maioria dos casos, você define os estilos para o modelo de seu componente em um arquivo separado.
```
  @Component({
    selector: 'app-component-overview',
    templateUrl: './component-overview.component.html',
    styleUrls: ['./component-overview.component.css']
  })
```
*  Adicione uma classinstrução que inclua o código do componente.
```
  export class ComponentOverviewComponent {}
```
