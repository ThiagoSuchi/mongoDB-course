# Introdução ao MongoDB

MongoDB é um banco de dados NoSQL orientado a documentos, conhecido por sua flexibilidade e escalabilidade. Em vez de armazenar dados em tabelas como os bancos relacionais, ele utiliza documentos no formato JSON (ou BSON internamente), o que o torna ideal para aplicações modernas que requerem estrutura de dados dinâmica e de fácil manipulação.

## Por que usar MongoDB?

- **Flexível**: Não requer esquemas rígidos, permitindo modelar dados de forma mais natural.
- **Escalável**: Suporta grandes volumes de dados e é fácil de escalar horizontalmente.
- **Alta Performance**: Ótimo para aplicações que necessitam de consultas rápidas e operações em tempo real.

## Principais Conceitos

- **Coleções**: Equivalem às tabelas em bancos de dados relacionais, mas armazenam documentos.
- **Documentos**: São registros armazenados em formato JSON, contendo pares de chave-valor.
- **Banco de Dados**: Contém várias coleções, é a estrutura mais alta de armazenamento.

---

## Comandos Essenciais do MongoDB

### 1. **Comandos Básicos**
| Comando                          | Descrição                                                                 |
|----------------------------------|---------------------------------------------------------------------------|
| `mongod`                         | Inicia o servidor MongoDB.                                                |
| `mongo`                          | Abre o shell interativo do MongoDB para executar comandos.                |
| `mongod --version`               | Mostra a versão instalada do MongoDB.                                     |

---

### 2. **Comandos de Banco de Dados**
| Comando                          | Descrição                                                                 |
|----------------------------------|---------------------------------------------------------------------------|
| `show dbs`                       | Lista todos os bancos de dados disponíveis.                               |
| `use <nome_banco>`               | Alterna para o banco de dados especificado ou o cria, caso não exista.    |
| `db`                             | Exibe o banco de dados atualmente selecionado.                            |
| `db.dropDatabase()`              | Remove o banco de dados atualmente selecionado.                           |

---

### 3. **Comandos de Coleções**
| Comando                          | Descrição                                                                 |
|----------------------------------|---------------------------------------------------------------------------|
| `show collections`               | Lista todas as coleções no banco de dados atual.                          |
| `db.createCollection("<nome>")`  | Cria uma nova coleção.                                                    |
| `db.<colecao>.drop()`            | Remove a coleção especificada.                                            |

---

### 4. **Comandos de Documentos**
| Comando                          | Descrição                                                                 |
|----------------------------------|---------------------------------------------------------------------------|
| `db.<colecao>.insertOne({})`     | Insere um único documento na coleção especificada.                        |
| `db.<colecao>.insertMany([{}])`  | Insere múltiplos documentos na coleção.                                   |
| `db.<colecao>.find()`            | Retorna todos os documentos da coleção.                                   |
| `db.<colecao>.findOne()`         | Retorna o primeiro documento encontrado na coleção.                       |
| `db.<colecao>.updateOne()`       | Atualiza o primeiro documento que atende ao filtro especificado.          |
| `db.<colecao>.updateMany()`      | Atualiza todos os documentos que atendem ao filtro especificado.          |
| `db.<colecao>.deleteOne()`       | Remove o primeiro documento que atende ao filtro especificado.            |
| `db.<colecao>.deleteMany()`      | Remove todos os documentos que atendem ao filtro especificado.            |

---

### 5. **Comandos de Indexação**
| Comando                          | Descrição                                                                 |
|----------------------------------|---------------------------------------------------------------------------|
| `db.<colecao>.createIndex({})`   | Cria um índice para otimizar buscas em campos específicos.                |
| `db.<colecao>.getIndexes()`      | Lista todos os índices definidos na coleção.                              |

---

### 6. **Outros Comandos Úteis**
| Comando                          | Descrição                                                                 |
|----------------------------------|---------------------------------------------------------------------------|
| `db.stats()`                     | Exibe estatísticas do banco de dados atual.                               |
| `db.<colecao>.stats()`           | Exibe estatísticas da coleção especificada.                               |
| `db.<colecao>.countDocuments()`  | Conta o número de documentos em uma coleção.                              |

---

## Recursos Adicionais

Para aprofundar seus conhecimentos no MongoDB, confira:
- [Documentação Oficial](https://www.mongodb.com/docs/)
- [MongoDB University](https://university.mongodb.com/)

Este README fornece uma visão geral para quem está começando com o MongoDB, mas há muito mais para explorar!
