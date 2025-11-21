## Cenário 01: Cadastros produtos fictícios via importação XML

### Caso de Teste 01: Cadastro via importação XML

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT01 | O usuario deve importar o XML.                           |

| **Pré-condições**                                                   |
| :------------------------------------------------------------       |
| O XML deve ser valido e não pode ser vazio.                         |

| **Passos**                                                          |
| :----------------------------------------------------------------   |
| **DADO** principal                                                  |
| **QUANDO** clica-mos em pedidos e escolhemos a opção "Importar XML de compra"                                                               |
| **ENTÃO** ira abrir a tela para importar o XML                      |
| **E** preenchemos os campos obrigatorios                            |
| **E** importamos o XML                                              |
| **QUANDO** clicarmos no botão "Gerar Compra"                        |
| **ENTÃO** a tela de compra sera exibida|

| **Critérios de aceitação**                                          |
| :--------------------------------------------------------------     |
| os registros dos produtos devem ser exibidos                        |
| [Video](https://drive.google.com/file/d/1JXvgGtODDgTwIiJn6S45O5uVAcHku3lI/view?usp=drive_link)                                                       |

---

### Caso de Teste 02: Tentativa de cadastro via importação XML vazio

| ID       | Descrição                                                                |
| :------- | :-------------------------------------------------------                 |
| C01-CT02 | Verificar se o sistema valida corretamente                               |

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
| [Video](https://drive.google.com/file/d/15_13DcOKZLeJeLkUVZ3PHwwwAlzNMKII/view?usp=drive_link)                                                                    |

---