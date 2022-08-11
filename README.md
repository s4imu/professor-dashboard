# Sistema de Notas

Esse projeto trata-se de um dashboard para professores cadastrarem seus alunos.

Resumo sobre o que aprendi nos cursos

Angular é framewrok do Javascript para aplicativos web SPA, também conhecidos como Single Pages Applications, baseados em componentes e que utiliza o Typescript para geração de seus módulos e componenentes. Atualmente ele está na versão 9 que trabalha principalmente com componentes.

Componente é um trecho de código que representa um componente visual da sua tela. Ele é composto por arquivos html(estrutura), css(estilo), ts(comportamento). Quando ele é criado uma tag é gerada que serve para referenciar o codigo html/css/ts criado no componente.

normalmente o nome dos arquivos criados seguem esse padrão:

home.component.css
home.component.html
home.component.ts

Temos um componente principal que referencia outros componentes (header, content, footer, etc...) os componentes sao organizados em modulos, e podemos construir componentes que estarão visiveis apenas dentro do modulo que foi criado ou visiveis para outros modulos.

Anatomia do modulo
Atributos
Declarations: components, derivas, pipes
Imports: module a/b/c
Exports: components, diretivas, pipes (para ser visível a outros módulos ele precisa tá aqui)
Providers: service A, B, C
Bootstrap: App Component (aponta para o componente que será carregado na app) 

Durante a inicialização o main.ts é chamado para inicializar a app em angular ele chama um modulo chamado AppModule: modulo de inicialização da aplicação que contém Bootstrap que aponta para Appcomponent: por onde a arvore de componentes sera chamada. 

Um Angular Decorator é uma função, usando a qual anexamos metadados a uma classe, método, acessador, propriedade ou parâmetro.

Temos dois tipos de diretivas:
Diretiva atributo: altera aparencia/comportamento de um elemento,componente ou outra diretiva
Diretiva estrutural: altera a estrutura da pagina adicionando/removendo elementos da DOM

Temos dois tipos de binding:
Bindiing de atributo: comunicação de atributos entre o TS e o HTML 
Binding de evento: ligar um evento entre html e ts

bindings podem ter as seguintes direções:
Binding de uma unica direção (one way data binding): alterações são aplicadas do sentido do TS para o HTML
Binding de uma dupla direção (two way data binding): alterações são aplicadas em ambos sentido TS para o HTML

Rotas: mapeamento entre rota e componente quando escolhido componente é selecionado no router outlet

Pipes:  Processamento em váriaveis, interpolações.

Programação Reativa: processamento ocorre quando ha a chamada do código
Padrão Observer: orientado a evento, Subject monitorar algo que acontece. Observer estao interessados que um evento aconteça subjecy  fica verificando caso algo esteja acontecendo e notificam os objects se acontecer 

Promises: encadeamento de chamadas usada uma unica vez. Padrão que era utilizado até pouco tempo atrás
Observables: função como parametro para outra função, callbacks. Reutilizavel, stream de dados e operadores (funções uitlizaveis). Código assincrono. 
 
Services:  classes para organização e compartilhamento de de metódos e dados entre componentes 

Injeção de dependencias: padrão no qual a classe recebe dependencias de fonte externa

