## Cenário 03: Editar produtos.

### Caso de Teste 01: Editar os campos do produto.

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C03-CT01 | Alterar os campos do produto.                            |

| **Pré-condições**                                                   |
| :------------------------------------------------------------       |
| Acessar tela de editar produtos.                                    |

| **Passos**                                                          |
| :----------------------------------------------------------------   |
| **DADO** que estamos na tela de editar produtos                     |
| **QUANDO** clicarmos no botão "Editar"                              |
| **ENTÃO** ira abrir a tela para editar produto                      |
| **E** alteramos os desejados campos corretamente                    |
| **QUANDO** clicarmos no botão "Salvar"                              |
| **ENTÃO** seremos redirecionados para a tela de cadastro de produtos|

| **Critérios de aceitação**                                          |
| :--------------------------------------------------------------     |
| Na tela principal deve estar listada os dados do produto editado    |
| [Video]([https://drive.google.com/file/d/1sBzoHoInLbVtbCQforKkxOhAYrWuHDHQ/view?usp=drive_link]())                                                    |

---

### Caso de Teste 02: Tentativa de edição de produto sem preencher os campos obrigatorios.

| ID       | Descrição                                                                |
| :------- | :-------------------------------------------------------                 |
| C03-CT02 | Verificar se o sistema valida corretamente.                              |

| **Pré-condições**                                                                   |
| :------------------------------------------------------------                       |
| O usuário deve deixar vazio os campos nome e grupo.                                 |

| **Passos**                                                                          |
| :----------------------------------------------------------------                   |
| **DADO** que estamos na tela para editar o produto                                  |
| **E** deixa-mos os campos "nome do produto" e "grupo" vazio                         |
| **QUANDO** clicarmos no botão "salvar"                                              |
| **ENTÃO** uma mensagem ira aparecer na tela obriganto o usuario a preencher o campo |

| **Critérios de aceitação**                                                          |
| :--------------------------------------------------------------                     |
| A mensagem de erro deve ser exibida.                                                |
| [Video]([https://drive.google.com/file/d/1NdKt2T8NZZGkXFkXicX_ZuNqBZUHKsDx/view?usp=drive_link]()) |

---