# Sobre
Estamos desenvolvendo as funcionalidades da aplicação “Gerenciador Financeiro” durante as aulas, o novo desafio será a evolução individual do sistema.

Um grande benefício dessa abordagem é a liberdade de execução das suas ideias. Você é livre para resolver a problemática da melhor maneira, se esta estiver dentro dos requisitos da atividade proposta.

1. Os exercícios de 6 a 10 resultarão na possibilidade de adicionar despesas divididas em um grupo de pessoas.
2. A resolução das atividades deve ter foco em utilizar, sempre que for conveniente:
   * POO (Classes, Atributos e Closure)
   * Métodos de arrays (evite seguir utilizando for para percorrer arrays)
3. Uma ideia de layout foi desenvolvida, você pode acessar [Gestor financeiro](https://www.figma.com/file/lVjA8As4wKdmjf48d79fwU/Gestor-financeiro?node-id=0%3A1&t=nc0wP9GP1TqFVilp-1) . Porém, neste momento tente ter maior ênfase em desenvolver as funcionalidades.
4. Para maior facilidade na execução dos exercícios, os faça em ordem.

## Lista dos exercícios

### Exercício 1
Crie uma nova página na aplicação para que as despesas em grupo sejam exibidas.

Esta página deve atender aos seguintes requisitos:

* Header com Botão de voltar (para voltar para a home), nome da página (Despesas em grupo) e ao lado botão para cadastro de nova despesa em grupo (por enquanto sem funcionalidade)
* O corpo da página deve estar pronto para exibir uma listagem de despesas em grupo onde haja um título para a despesa, o valor repartido em partes iguais para o grupo e por fim o valor final da despesa;
* Crie uma classe para criar o objeto de despesa em grupo, o qual deve conter as seguintes propriedades:
* Título que descreva a despesa (title)
* Valor parcial, a parte de cada um na despesa (partialValue)
* Em quantas pessoas o valor deve ser dividido, é uma propriedade privada (numberOfParticipants)
* O valor total da despesa (amount)
* Por enquanto use um array com dados fictícios, o cadastro de valores será contruído na próxima tarefa.

### Exercício 2

Crie um botão para exibir um modal para cadastro de despesas em grupo. Ao clicar no botão um modal deve ser aberto (conforme ocorre atualmente no sistema para cadastro de despesas individuais).

O modal aberto deve possuir um formulário com os seguintes campos:

* Título que descreva a despesa (title)
* Em quantas pessoas o valor deve ser dividido (numberOfParticipants)
* O valor total da despesa (amount)
* Abaixo do formulário deve haver um botão “Adicionar”, que ao ser clicado deve adicionar a despesa na lista de despesas (Array.push).

### Exercício 3

No clique do botão “Adicionar” você adicionou a despesa a listagem sem o cálculo do valor parcial. Mas, como você tem o valor total e o número de pessoas que irão dividir a despesa calcule o valor parcial (a parte de cada um)

### Exercício 4

Crie um menu, ou botão para que o usuário possa navegar entre as despesas individuais e em grupo. Não esqueça de pensar nos dois caminhos:

* Despesas Individuais → Despesas em grupo
* Despesas em grupo → Despesas individuais

Use sua criatividade no layout.

### Exercício 5

Sempre que uma despesa em grupo for adicionada adicione um alert para que o usuário seja notificado de que a ação dele funcionou.