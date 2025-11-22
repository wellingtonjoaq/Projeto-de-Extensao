## Cenário 01: Fechamento Caixa

### Caso de Teste 01: Simular operações de 1 caixa (Não e possivel simular 3 caixas!).

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT01 |  Abrir operação de 1 caixa                               |

| **Pré-condições**                                                   |
| :------------------------------------------------------------       |
|  Estar logado com um usuario no sistema                             |

| **Passos**                                                          |
| :----------------------------------------------------------------   |
| **DADO** que estou na tela "Livro do caixa"                         |
| **QUANDO** clico em abrir caixa                                     |
| **ENTÃO** o sistema exibe uma tela para por saldo do caixa          |
| **E** informo o saldo                                               |
| **QUANDO** clico em "Salvar"                                        |
| **ENTÃO** o caixa e aberto e é listado o registro dele              |

| **Critérios de aceitação**                                          |
| :--------------------------------------------------------------     |
|  Caixa deve estar abrir com sucesso.                                |
| [Video](https://drive.google.com/file/d/1EvP-vxHBiPbQHGXQdWlplTMAK_IKwUl9/view?usp=drive_link)                                                    |

---

### Caso de Teste 02: Gerar vendas com tipos de documentos 

| ID       | Descrição                                                                                       |
| :------- | :-------------------------------------------------------                                        |
| C01-CT02 |  Gerar 3 tipos de documentos                                                                    |

| **Pré-condições**                                                                                          |
| :------------------------------------------------------------                                              |
|  compra status "Não confirmada"                                                                            |

| **Passos**                                                                                                 |
| :----------------------------------------------------------------                                          |
| **DADO** que estou na tela "Confirmar Venda"                                                               |
| **QUANDO** clico no icone de "Arquivo"                                                                     |
| **ENTÃO** o sistema exibe uma tela para informar o tipo de documento                                       |
| **E** preencho todos os campos do tipo de documento com valor inferior ao valor total da venda             |
| **QUANDO** quando clico em "Salvar"                                                                        |
| **ENTÃO** abre uma tela de confirmação                                                                     |
| **QUANDO** quando clico em "Confirmar"                                                                     |
| **ENTÃO** volto para tela de "Confirmar Venda" com o documento listado                                     |
| **E** repito todo esse ciclo mais 2 vezes ate dar o valor total da venda com tipos de documento diferentes |
| **QUANDO** quando clico em "Salvar"                                                                        |
| **ENTÃO** volto para tela de "Venda" com o status de venda "Confirmada"                                    |

| **Critérios de aceitação**                                                                                 |
| :--------------------------------------------------------------                                            |
|  A mensagem de venda finalizada so deve ser exibida se clicar em finalizar                                 |
| [Video](https://drive.google.com/file/d/1_7JWx7xAUo6QpnXwlVIocjRdtOK2cluP/view?usp=drive_link)                                                                                              |

---

### Caso de Teste 03: Gerar vendas com tipos de documentos vazio

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT03 |  Abrir operação de 1 caixa                               |

| **Pré-condições**                                                   |
| :------------------------------------------------------------       |
|  Estar logado com um usuario no sistema                             |

| **Passos**                                                          |
| :----------------------------------------------------------------   |
| **DADO** que estou na tela "Livro do caixa"                         |
| **QUANDO** clico em abrir caixa                                     |
| **ENTÃO** o sistema exibe uma tela para por saldo do caixa          |
| **E** informo o saldo                                               |
| **QUANDO** quando clico em "Salvar"                                 |
| **ENTÃO** o caixa e aberto e é listado o registro dele              |

| **Critérios de aceitação**                                          |
| :--------------------------------------------------------------     |
|  Caixa deve estar aberto.                                           |
| [Video](https://drive.google.com/file/d/1AJvXuW7bgheziF1pvjCt_9JsrT-YhPv6/view?usp=drive_link)                                                    |

---

### Caso de Teste 04: Realizar retirar valores 

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT04 |  Abrir operação de 1 caixa                               |

| **Pré-condições**                                                   |
| :------------------------------------------------------------       |
|  Estar logado com um usuario no sistema                             |

| **Passos**                                                          |
| :----------------------------------------------------------------   |
| **DADO** que estou na tela "Livro do caixa"                         |
| **QUANDO** clico em abrir caixa                                     |
| **ENTÃO** o sistema exibe uma tela para por saldo do caixa          |
| **E** informo o saldo                                               |
| **QUANDO** quando clico em "Salvar"                                 |
| **ENTÃO** o caixa e aberto e é listado o registro dele              |

| **Critérios de aceitação**                                          |
| :--------------------------------------------------------------     |
|  Caixa deve estar aberto.                                           |
| [Video](https://drive.google.com/file/d/161RrIVrSG5Tj6gbZ2LGg8cnxHe0xkB1V/view?usp=drive_link)                                                    |

---

### Caso de Teste 05: Retirar valor invalido

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT05 |  Abrir operação de 1 caixa                               |

| **Pré-condições**                                                   |
| :------------------------------------------------------------       |
|  Estar logado com um usuario no sistema                             |

| **Passos**                                                          |
| :----------------------------------------------------------------   |
| **DADO** que estou na tela "Livro do caixa"                         |
| **QUANDO** clico em abrir caixa                                     |
| **ENTÃO** o sistema exibe uma tela para por saldo do caixa          |
| **E** informo o saldo                                               |
| **QUANDO** quando clico em "Salvar"                                 |
| **ENTÃO** o caixa e aberto e é listado o registro dele              |

| **Critérios de aceitação**                                          |
| :--------------------------------------------------------------     |
|  Caixa deve estar aberto.                                           |
| [Video](https://drive.google.com/file/d/11HAXJVYcQqHK4lqGae2w9Asj4AdDMeNj/view?usp=drive_link)                                                    |

---

### Caso de Teste 06: Fechar o caixa e conferir os tipos de documentos

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT06 |  Abrir operação de 1 caixa                               |

| **Pré-condições**                                                   |
| :------------------------------------------------------------       |
|  Estar logado com um usuario no sistema                             |

| **Passos**                                                          |
| :----------------------------------------------------------------   |
| **DADO** que estou na tela "Livro do caixa"                         |
| **QUANDO** clico em abrir caixa                                     |
| **ENTÃO** o sistema exibe uma tela para por saldo do caixa          |
| **E** informo o saldo                                               |
| **QUANDO** quando clico em "Salvar"                                 |
| **ENTÃO** o caixa e aberto e é listado o registro dele              |

| **Critérios de aceitação**                                          |
| :--------------------------------------------------------------     |
|  Caixa deve estar aberto.                                           |
| [Video](https://drive.google.com/file/d/1LFVvmw_Q7GvdR8g7z14n6RmMaolfJEgm/view?usp=drive_link)                                                    |

---

### Caso de Teste 07: Conciliar totais com relatório de vendas

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT07 |  Abrir operação de 1 caixa                               |

| **Pré-condições**                                                   |
| :------------------------------------------------------------       |
|  Estar logado com um usuario no sistema                             |

| **Passos**                                                          |
| :----------------------------------------------------------------   |
| **DADO** que estou na tela "Livro do caixa"                         |
| **QUANDO** clico em abrir caixa                                     |
| **ENTÃO** o sistema exibe uma tela para por saldo do caixa          |
| **E** informo o saldo                                               |
| **QUANDO** quando clico em "Salvar"                                 |
| **ENTÃO** o caixa e aberto e é listado o registro dele              |

| **Critérios de aceitação**                                          |
| :--------------------------------------------------------------     |
|  Caixa deve estar aberto.                                           |
| [Video](https://drive.google.com/file/d/1_61e62x5oH0vyr63UAaBMdonC9XOspBC/view?usp=drive_link)                                                    |

---