# DiarioDeBordoMRelacional

## Como organizamos os dados em tabelas
É a representação genérica de um componente do mundo real, sobre o qual desejamos armazenar informações, uma representação de quase todas as informações com varias propriedades que devem ser compreendidas pelo sistema de informação, qualquer coisa que produza ou consuma informações. Entidade são coisas significativas sobre a qual a organização deseja guarda, ou seja, (coletar, manter e etc) dados podendo ser algo tangível ou intangível.
- todos os elementos que tenham existência concreta. Fisicamente existente. Ex: Produto, animal, carro.
- todo o tipo de papel, atribuição, classificação, capacitação, ou outra característica que especifique atuação. Ex: Cliente, professor, departamento.
- só conseguem ser percebidos ou caracterizados, enquanto uma certa ação se desenrola. Ex: Lançamento em conta corrente.

[fonte](https://www.devmedia.com.br/modelagem-relacional/19614)

## Oque são PK e FK
### Primary Key (Chave Primaria)
É o conceito mais básico relacionado à organização em um banco de dados. Toda tabela possuirá uma, e somente uma
identificador único da tabela, sendo representado por aquele campo (ou campos) que não receberá valores repetidos.

características:
- não pode ser nula
- cada registro deve possuir uma, somente uma
- são incrementadas automaticamente pelo banco de dados (não usa INSERT)
- são para o relacionamento entre entidades, haverá relacionada uma referência: Chave Estrangeira (FK)

### Foreign Key (Chave estrangeira)
Ela diz respeito a um relacionamento entre tabelas
é uma referência em uma tabela a uma chave primária de outra tabela
ela sinaliza/referência a PK nela mesma

### Diferenças entre PK a FK
- Pode ser nula (NOT NULL)
- é um campo em uma tabela que faz referência a um campo que é chave primária em outra tabela
- é possível ter mais de uma (ou nenhuma) em uma tabela

alerta: embora não haja, efetivamente, nenhum problema das chaves estrangeiras aceitarem o valor null, tal característica pode gerar o que é chamado de registro órfão, isto é, um registro sem dados para um determinado relacionamento.

[fonte PK e FK](https://www.devmedia.com.br/sql-aprenda-a-utilizar-a-chave-primaria-e-a-chave-estrangeira/37636)

## Como o modelo lógico se diferencia do conceitual?

# Modelo Conceitual
Modelo que representa fielmente o negocio em questão, demonstrando características fieis ao ambiente observado ou imaginado independente de qualquer limitação imposta por tecnologia, técnica de implementação ou dispositivo físico.
Deve ser utilizada na fase de analise, nunca na fase de projeto, em nível de conversação, representação do negocio, validação de conceitos etc.
**Um grande diferencial do modelo conceitual é sua estabilidade, pois permanece sem mudanças independente da escolha futura de implementação, em um SGBD relacional ou um hierárquico**

# Modelo Lógico
Ao contrário dos modelos conceituais, os modelos lógicos são os modelos em que os objetos, suas características e relacionamentos têm sua representação de acordo com as regras de implementação e limitantes impostos por alguma tecnologia
**esse modelo será criado através do modelo conceitual já construído, teoria essa que alguns autores têm uma visão diferenciada, definindo que o método para obtenção do modelo lógico é o próprio processo criativo, sem haver a necessidade de um modelo conceitual.**
