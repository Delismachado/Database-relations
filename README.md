### Desafio-09-Database-relations
Neste desafio do curso GoStack da Rocketseat, fiz uma aplicação usando Node.js e TypeScript, incluindo o uso de banco de dados com o TypeORM,
com relacionamentos ManyToMany!

#### A principal atividade foi criar rotas na aplicação:

- POST: A rota deve receber name e email dentro do corpo da requisição, sendo o name o nome do cliente a ser cadastrado.
Ao cadastrar um novo cliente, ele deve ser armazenado dentro do seu banco de dados e deve ser retornado o cliente criado.
Ao cadastrar no banco de dados, na tabela customers deverá possuir os campos name, email, created_at, updated_at.

- POST: Essa rota deve receber name, price e quantity dentro do corpo da requisição, sendo o name o nome do produto a ser cadastrado,
price o valor unitário e quantity a quantidade existente em estoque do produto. Com esses dados devem ser criados no banco de dados um novo
produto com os seguintes campos: name, price, quantity, created_at, updated_at.

- POST /orders/: Nessa rota você deve receber no corpo da requisição o customer_id e um array de products, contendo o id e a quantity que você deseja
adicionar a um novo pedido. Aqui você deve cadastrar na tabela order um novo pedido, que estará relacionado ao customer_id informado, created_at e
updated_at . Já na tabela orders_products, você deve armazenar o product_id, order_id, price e quantity, created_at e updated_at.

#### OBS: Para o desenvolvimento da aplicação usei o Insomnia para testar as rotas criadas!! 

## Links úteis para desenvolver uma aplicação como esta:
- <p>Rocketseat: <a href="http://example.com/" title="Title">https://rocketseat.com.br/</a></p>
- <p>Insomnia: <a href="http://example.com/" title="Title">https://insomnia.rest/</a></p>
- <p>Cascade option TypeORM: <a href="http://example.com/" title="Title">https://github.com/typeorm/typeorm/blob/master/docs/relations.md#cascade-options</a></p>
- <p>Relacionamento many-to-many personalizado: <a href="http://example.com/" title="Title">https://github.com/typeorm/typeorm/blob/master/docs/many-to-many-relations.md#many-to-many-relations-with-custom-properties</a></p>
- <p>Eager loading com TypeORM: <a href="http://example.com/" title="Title">https://github.com/typeorm/typeorm/blob/master/docs/eager-and-lazy-relations.md#eager-relations</a></p>
- <p>Opções de relacionamentos do TypeORM: <a href="http://example.com/" title="Title">https://github.com/typeorm/typeorm/blob/master/docs/find-options.md</a></p>

