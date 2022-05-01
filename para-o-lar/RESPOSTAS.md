# Respostas

1. Qual nivel de maturidade corresponde ao CRUD (Create, Read, Update, Delete)?
R = API REST Maturidade 2

2. Qual a relação entre os metodos HTTP e o CRUD?
R= Os verbos HTTP parecem estar diretamente ligado com o CRUD:

Create -> POST
Read -> GET
Update -> PUT / PATCH
Delete -> DELETE
Por causa de uma confusão na classificação de Resource, acabam relacionando REST diretamente a um CRUD. Por causa desse erro de classificação, quem busca criar api's verdadeiramente RESTFul terá dificuldades em seguir as "bases" do conceito devido a essa similiaridade.

3. O que é HATEOAS? Ele é obrigatório para que uma API seja considerada RESTfull?

R= HATEOAS é um componente que faz parte da arquitetura REST, cujo objetivo é ajudar os clientes a consumirem uma API sem a necessidade de conhecimento prévio.
Os principais critérios para uma API ser RESTful são:
Uniform Interface;
Stateless;
Cacheable;
Client-Server;
Layered system.
Sem seguir todas estas restrições, sua API não será RESTful, será apenas mais uma implementação RPC em cima do protocolo HTTP.

4. O que quer dizer quando dizemos que uma API é idempotente?

R = Um método HTTP é idempotente se uma requisição idêntica pode ser feita uma ou mais vezes em sequência com o mesmo efeito enquanto deixa o servidor no mesmo estado. Em outras palavras, um método idempotente não deveria possuir nenhum efeito colateral (exceto para manter estatísticas).

5. Qual a diferença entre os métodos PUT e PATCH?

R = O método de requisição HTTP PATCH aplica modificações parciais a um recurso. O método HTTP PUT permite apenas substituições completas de um documento. Em contraste ao PUT , o método PATCH não é idempotente, ou seja, requisições sucessivas idênticas podem obter efeitos distintos.
