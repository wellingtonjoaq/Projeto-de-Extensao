## Cenário 04: Buscar Produto.

### Caso de Teste 01: Vereficar se consigo buscar o produto desejado.

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C02-CT04 | Verificar se consigo buscar o produto                    |

| **Pré-condições**                                                   |
| :------------------------------------------------------------       |
| Devo informar o nome do produto ja cadastrado para buscar           |

| **Passos**                                                          |
| :----------------------------------------------------------------   |
| **DADO** que estamos na tela de cadastro de produtos                |
| **QUANDO** clicarmos no botão com icone de "Lupa"                   |
| **ENTÃO** ira abrir uma tela de busca      |
| **E** Insirimos o nome do produto no campo "contendo".              |
| **QUANDO** clicarmos no botão "Pesquisar"                           |
| **ENTÃO** o sistema ira retornar o produto com o nome informado     |

| **Critérios de aceitação**                                          |
| :--------------------------------------------------------------     |
| O produto informado deve ser exibido corretamente.                  |
| [Video]([https://drive.google.com/file/d/1SGMzX-t-qfG5wQvCe-npcxw9hqN4VgjT/view?usp=drive_link]()) |

---

### Caso de Teste 02: Buscar produto inexistente.

| ID       | Descrição                                                  |
| :------- | :-------------------------------------------------------   |
| C02-CT04 | Verificar se o sistema não puxa um registro inexistente    |

| **Pré-condições**                                                     |
| :------------------------------------------------------------         |
| Devo informar o nome do produto inexistente para buscar               |

| **Passos**                                                            |
| :----------------------------------------------------------------     |
| **DADO** que estamos na tela de cadastro de produtos                  |
| **QUANDO** clicarmos no botão com icone de "Lupa"                     |
| **ENTÃO** ira abrir uma tela de busca      |
| **E** Insirimos o nome de um produto inexistente no campo "contendo". |
| **QUANDO** clicarmos no botão "Pesquisar"                             |
| **ENTÃO** o sistema ira retornar nada                                 |

| **Critérios de aceitação**                                            |
| :--------------------------------------------------------------       |
| O sistema não deve encontrar nada                                     |
| [Video]([https://drive.google.com/file/d/1hEisASdDnP_rvLiaFOsHZlPog1FL7XK5/view?usp=drive_link]()) |

---