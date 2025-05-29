## Projeção
- Prof vai passar lição de certificado em oracle
## Produto Cartesiano
- Junção de uas tabelas sem inner join
- funcionario x cargo

---
## Operações Relacionais
### Minus
- Tudo que está em um que não está na outra
- "Trazer todo mundo da A que não está na B"
### Union
- Pega tudo de todas as tabelas
- Se quero ver todos os dados é Union All, o Union padrão ignorou o
- Union: Se achar o mesmo conjuto de dados, ele não traz
- Union All: Traz os dados mesmo repetidos 
### Intersecção
- Tudo que elas tem em comum
- "Ela vai comparar oq vc trouxe no seu Select"
### Junção
- "E tem junção que tem esse simboloBla bla bla" - Cristiane Palomar
---
## Oracle
### Porque não deu certo o Union?
- Union voce precisa de dois conjunto de dados, e faz dois selects
- A quantidade de campos de A tem que ser o mesmo de B
- Não pode pegar 5 de uma e 3 de outra, tem que ser a mesma quantia e tipos de dados

---
## "Se eu pedir na prova vocês sabem fazer?"
1. Modify no Alter Table
2. Não pode trazer as explicações em papel, só o comando
3. "Já viram insert com select"

## Codigo da Aula
```
-- Union -- Intersect -- Minus --
select codcliente, nome from cliente
UNION
select codcliente, nmcliente from exclientes

delete from ecclientes
alter table exclientes
modify codcliente number;

insert into exclientes (codcliente, nmcliente)
values(10099, 'Sophia')
```
