## Cenário 02: Gerar vendas com tipos de documentos 

### Caso de Teste 01: Gerar vendas com tipos de documentos.

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT01 | Criar vendas com varios tipos de documentos              |

| **Pré-condições**                                                   |
| :------------------------------------------------------------       |
| o usuario deve cadastrar 3 tipos de documentos                      |

| **Passos**                                                          |
| :----------------------------------------------------------------   |
| **DADO** que estou na tela de venda                                 |
| **QUANDO** clico em "Novo"                                          |
| **ENTÃO**  abre a tela para cadastrar venda                         |
| **E** devo selecionar cliente, funcionario e produto                |
| **QUANDO** cadastro a venda e clico em finalizar                    |
| **ENTÃO** a tela de finalizar venda e exibida                       |
| **E** devo preencher 3 tipos de documento                           |
| **QUANDO** clico em "Salvar"                                        |
| **ENTÃO** a tela de finalizar venda e exibida com status de confirmada                                                            |

| **Critérios de aceitação**                                          |
| :--------------------------------------------------------------     |
|  o status da compra deve estar confirmada           |
| [Video]([]())                                                    |

---