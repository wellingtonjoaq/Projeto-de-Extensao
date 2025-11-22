## Cenário 01: Processamento de Venda (PDV)

### Caso de Teste 01: Iniciar nova venda com 5 itens

| ID       | Descrição                                                       |
| :------- | :-------------------------------------------------------        |
| C01-CT01 | Iniciar venda com 5 itens                                       |

| **Pré-condições**                                                          |
| :------------------------------------------------------------              |
| Acessar tela de venda.                                                     |

| **Passos**                                                                 |
| :----------------------------------------------------------------          |
| **DADO** que estamos na tela de venda                                      |
| **QUANDO** clicarmos no botão "Novo"                                       |
| **ENTÃO** ira abrir a tela para cadastrar o cliente e funcionario da venda |
| **E** preenchemos todos campos corretamente                                |
| **QUANDO** clicarmos no botão "Salvar"                                     |
| **ENTÃO** a tela de entrada de produto sera aberta                         |
| **E** preenchemos todos campos corretamente                                |
| **QUANDO** clicarmos no botão "Salvar"                                     |
| **ENTÃO** ira abrir a tela de venda com o produto informado                |
| **ENTÃO** agora repita e ciclo mais 4 vezes                                |

| **Critérios de aceitação**                                                 |
| :--------------------------------------------------------------            |
| Na tela de venda deve ter 5 itens listados                                 |
| [Video](https://drive.google.com/file/d/1f8zZzjTe757E3Vjmdtrc4WL9lc9J967u/view?usp=drive_link)                                                              |

---

### Caso de Teste 02: Tentativa de iniciar venda sem preencher os campos obrigatorios.

| ID       | Descrição                                                       |
| :------- | :-------------------------------------------------------        |
| C01-CT02 | Verificar bloqueia campos vazios em campos obrigatorios         |

| **Pré-condições**                                                          |
| :------------------------------------------------------------              |
| O usuário não deve preencher os campos obrigatorios.                       |

| **Passos**                                                                 |
| :----------------------------------------------------------------          |
| **DADO** que estamos na tela de venda                                      |
| **QUANDO** clicarmos no botão "Novo"                                       |
| **ENTÃO** ira abrir a tela para cadastrar o cliente e funcionario da venda |
| **E** não preenchemos os campos obrigatorios                               |
| **QUANDO** clicarmos no botão "Salvar"                                     |
| **ENTÃO** mensagem de erro aparece na tela                                 |
| **E** preenchemos os campos corretamente                            |
| **QUANDO** clicarmos no botão "Salvar"                                     |
|**ENTÃO** a tela de entrada de produto sera aberta                          |
| **E** não preenchemos os campos obrigatorios                               |
| **QUANDO** clicarmos no botão "Salvar"                                     |
| **ENTÃO** mensagem de erro aparece na tela                                 |
| **E** preenchemos os campos corretamente                            |
| **QUANDO** clicarmos no botão "Salvar"                                     |
| **ENTÃO** ira abrir a tela de venda com o produto informado                |

| **Critérios de aceitação**                                                 |
| :--------------------------------------------------------------            |
| A mensagem de erro deve informar em qual campo foi.                        |
| [Video](https://drive.google.com/file/d/1n5F5NseSv4eSaHR2gndCPxolGaKndVZX/view?usp=drive_link)                                                              |

---

### Caso de Teste 03: Finalizar venda com pagamento misto (cartão 70% +
### dinheiro 30%)

| ID       | Descrição                                                       |
| :------- | :-------------------------------------------------------        |
| C01-CT03 | Finalizar venda com pagamento misto                             |

| **Pré-condições**                                                          |
| :------------------------------------------------------------              |
| O usuário deve registrar dois tipos de documento                           |

| **Passos**                                                                 |
| :----------------------------------------------------------------          |
| **DADO** que estamos na tela de venda                                      |
| **QUANDO** clicarmos no botão "Finalizar"                                  |
| **ENTÃO** a tela de confirmar venda e aberta                               |
| **E** definimos o status da venda como confirmada                          |
| **QUANDO** clicarmos no botão com icone de "Arquivo"                       |
| **ENTÃO** a tela de entrada de tipo de documento e aberta                  |
| **E** informa-mos os dados do documento                                    |
| **QUANDO** clicarmos no botão "Salvar"                                     |
| **ENTÃO** voltamos a tela de confirmar venda                               |
| **QUANDO** clicarmos no botão "Salvar"                                     |
| **ENTÃO** a venda e confirmada e volta para a tela de venda                |
| **QUANDO** clicarmos no botão "Finalizar"                                  |
| **ENTÃO** o sistema exibe a mensagem de "Venda Finalizada"                 |

| **Critérios de aceitação**                                                 |
| :--------------------------------------------------------------            |
| A mensagem de "Venda Finalizada" so deve ser exibida quando clicar no botão "Finalizar".                                                                 |
| [Video](https://drive.google.com/file/d/1pMaIGy4W9t4h4cp4vjI6xb7LmzHLRtAE/view?usp=drive_link)                                                              |

---

### Caso de Teste 04: Fechamento de caixa e validação por tipo de documento

| ID       | Descrição                                                        |
| :------- | :-------------------------------------------------------         |
| C01-CT04 | Fechamento de caixa                                              |

| **Pré-condições**                                                           |
| :------------------------------------------------------------               |
| O usuário deve estar com o caixa aberto.                                    |

| **Passos**                                                                  |
| :----------------------------------------------------------------           |
| **DADO** que estamos na tela de "Livro Caixa"                               |
| **QUANDO** clicarmos no botão "Fechar Caixa"                                |
| **E** seleciona-mos a opção fechar caixa                                    |
| **ENTÃO** a tela de "Fechamento de Caixa" e aberta                          |
| **E** visualiza-mos os dados                                                |
| **QUANDO** clicarmos no botão "Salvar"                                      |
| **ENTÃO** volta-mos para tela "Livro Caixa" com o registro do caixa fechado |

| **Critérios de aceitação**                                                  |
| :--------------------------------------------------------------             |
| O registro do caixa fechado deve ser mostrado na listagem                   |
| [Video](https://drive.google.com/file/d/1HsXCEk3h_wWf7k0FwP-StpizTSC2i0En/view?usp=drive_link)                                                               |

---