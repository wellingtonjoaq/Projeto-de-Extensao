## Cenário 07: Cadastro de produtos.

### Caso de Teste 01: produto com campos preenchidos corretamente.

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C07-CT01 | O cadastro deve ser preenchidos corretamente.            |

| **Pré-condições**                                                   |
| :------------------------------------------------------------       |
| Acessar tela de cadastro de produtos.                               |

| **Passos**                                                          |
| :----------------------------------------------------------------   |
| **DADO** que estamos na tela de cadastro de produtos                |
| **QUANDO** clicarmos no botão "Novo"                                |
| **ENTÃO** ira abrir a tela para cadastrar o produto                 |
| **E** preenchemos todos campos corretamente                         |
| **QUANDO** clicarmos no botão "Salvar"                              |
| **ENTÃO** seremos redirecionados para a tela de cadastro de produtos|

| **Critérios de aceitação**                                          |
| :--------------------------------------------------------------     |
| Na tela principal deve estar listada os dados do produto            |
| [Video]([https://drive.google.com/file/d/1TxVgQprg1wKJMuXNlSIelVGABuoopCIm/view?usp=drive_link]())                                                    |

---

### Caso de Teste 02: Tentativa de cadastro de produto sem preencher os campos obrigatorios.

| ID       | Descrição                                                                |
| :------- | :-------------------------------------------------------                 |
| C07-CT02 | Verificar se o sistema valida corretamente                               |

| **Pré-condições**                                                                   |
| :------------------------------------------------------------                       |
| O usuário não deve preencher os campos nome e grupo.                                |

| **Passos**                                                                          |
| :----------------------------------------------------------------                   |
| **DADO** que estamos na tela para cadastrar o produto                               |
| **E** deixa-mos os campos "nome do produto" e "grupo" vazio                         |
| **QUANDO** clicarmos no botão "salvar"                                              |
| **ENTÃO** uma mensagem ira aparecer na tela obriganto o usuario a preencher o campo |

| **Critérios de aceitação**                                                          |
| :--------------------------------------------------------------                     |
| A mensagem de erro deve ser exibida.                                                |
| [Video]([https://drive.google.com/file/d/1t1edldI-p6G237wb34n5IdzUi8BVVNjC/view?usp=drive_link]())                                                                    |

---