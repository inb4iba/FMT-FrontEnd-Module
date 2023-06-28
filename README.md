# Blog
Dessa vez iremos criar um Blog.

1. Os exercícios resultarão em um blog baseado na API [JsonPlaceholder](https://jsonplaceholder.typicode.com/).
2. A resolução das atividades deve ter foco em utilizar, sempre que for conveniente:
   * Async
   * Promises
   * Operadores Rest e Spread
3. Para maior facilidade na execução dos exercícios, os faça em ordem.
4. A documentação completa da API que vamos utilizar nesta semana está disponível [AQUI](https://github.com/typicode/json-server).
5. Na descrição das atividades há uma explicação/ideia de como implementar cada funcionalidade no projeto, mas sinta-se a vontade para utilizar sua própria metodologia nas implementações.

## Lista de Exercícios

### Exercício 1

* Crie os arquivos HTML, CSS e Javascript para a página home;
* No Javascript faça um fetch para o endpoint https://jsonplaceholder.typicode.com/posts?_page=1&_limit=20;
* Crie a estilização da página inicial do seu blog e exiba a listagem de posts que você carregou até então;
  
### Exercício 2

Ainda na home do seu blog, você pode imaginar que não mostrará apenas 20 posts para o usuário.

* Adicione um botão ao final da exibição dos posts, para que seja carregada a próxima página do endpoint ao clicar nele;
* Transforme os query params utilizados na requisição (page e limit) de posts em variáveis;
* Mude a string do endpoint de aspas simples para crase, para que possamos usar as váriaveis criadas como valores dos querys params;
  * ```https://jsonplaceholder.typicode.com/posts?_page=${postsPage}&_limit=${postsLimit}```
* Por padrão o botão de carregar mais posts deve estar com display none;
* Adicione uma condicional ao fim de cada requisição de posts para testar se a quantidade de posts recebida é a mesma que definimos como limite da requisição, no caso 20, se for a mesma significa que há mais resultados, então deixe o botão de carregar mais com display block e caso contrário com display none;
* Verifique se a paginação dos seus posts está funcionando corretamente;

### Exercício 3

Ao clicar em um post iremos abrir um modal que irá trazer todos os detalhes do post, que no caso são title, body ans comments. Para isso precisamos carregar seus comentários e exibir isso em um modal;

Uma das maneiras de lidar com este dinamismo é fazendo com que ao clicar em um post, uma função que receba como parâmetro o id, o body e o title do post atual, carregue os comentários consultando o endpoint de comentários e defina um objeto que contenha as informações correntes do post (body, title e id) e uma nova propriedade (comments) com os comentários recém carregados para que este seja o corpo do modal.;

* Crie uma variável para armazenar o post mais recente clicado (cou chamar de currentPost para poder fazer referência);
* Crie uma função que receba como parâmetro um id de post e faça uma consulta ao endpoint de comentários usando este id. O endpoint é: https://jsonplaceholder.typicode.com/posts/${postId}/comments;
* Retorne os comentários;
* Teste a função de busca de comentários;
* Crie uma função que receba como parâmetro id, body e title (de um post) e a partir disso carregue os posts usando a função do tópico 2, além disso, defina o calor da variável currentPost para os valores recebidos como parâmetro id, body, title e comments que foi carregado agora;

### Exercício 4

Ao clicar em um post iremos abrir um modal que irá trazer todos os detalhes do post, que no caso são title, body ans comments. Para isso precisamos carregar seus comentários e exibir isso em um modal;

Uma das maneiras de lidar com este dinamismo é fazendo com que ao clicar em um post, uma função que receba como parâmetro o id, o body e o title do post atual, carregue os comentários consultando o endpoint de comentários e defina um objeto que contenha as informações correntes do post (body, title e id) e uma nova propriedade (comments) com os comentários recém carregados para que este seja o corpo do modal.;

* Na função que você usou para criar cada post no html, defina para cada um a propriedade onclick que irá chamar a função criada no tópico 4;
* Verifique se ao clicar em um comentário os comentários dele são carregados e a variável currentPost é alterada;
* Crie um modal que exiba título, corpo e comentários de um post;
* Estilize o modal da maneira que preferir;
* Adicione ao fim da função do tópico 4 da parte 1, os comandos para que altere o “innerHTML" dos elementos de título, corpo e comentários do modal que você criou no tópico 3 desta parte;
* Por fim, após as definições do tópico 5 desta parte 2, abra o modal;

## Sobre

Além do requisitado, também adicionei um intersectionObserver para carregar mais posts quando o usuário chegar no último.

## Rodando o projeto

Você pode executar o projeto utilizando a extensão [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)  para VS Code ou qualquer outra similar, já que ele usa JS modular.

## Tecnologias

* HTML
* CSS
* JS

## Recursos

https://loading.io/css/