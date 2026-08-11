# DiarioDeBordoMRelacional

## Como organizamos os dados em tabelas

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
