## Cenário 01: Inventário de Estoque

### Caso de Teste 01: Cadastro via importação XML

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT01 | O usuario deve importar o XML.                           |

| **Pré-condições**                                                   |
| :------------------------------------------------------------       |
| O XML deve ser valido e não pode ser vazio.                         |

| **Passos**                                                          |
| :----------------------------------------------------------------   |
| **DADO** que estamos na tela principal                              |
| **QUANDO** clica-mos em pedidos e escolhemos a opção "Importar XML de compra"                                                               |
| **ENTÃO** ira abrir a tela para importar o XML                      |
| **E** preenchemos os campos obrigatorios                            |
| **QUANDO** clicarmos no botão "Importar XML"                        |
| **E** importamos o XML                                              |
| **QUANDO** clicarmos no botão "Gerar Compra"                        |
| **ENTÃO** a tela de compra sera exibida|

| **Critérios de aceitação**                                          |
| :--------------------------------------------------------------     |
| os registros dos produtos devem ser exibidos                        |
| [Video](https://drive.google.com/file/d/1JXvgGtODDgTwIiJn6S45O5uVAcHku3lI/view?usp=drive_link)                                                       |

---

### Caso de Teste 02: Tentativa de cadastro via importação XML vazio

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT02 | Verificar se o sistema não permite XML vazio             |

| **Pré-condições**                                                   |
| :------------------------------------------------------------       |
| O XML deve estar vazio                                              |

| **Passos**                                                          |
| :----------------------------------------------------------------   |
| **DADO** que estamos na tela principal                              |
| **QUANDO** clica-mos em pedidos e escolhemos a opção "Importar XML de compra"                                                               |
| **ENTÃO** ira abrir a tela para importar o XML                      |
| **E** preenchemos os campos obrigatorios                            |
| **QUANDO** clicarmos no botão "Importar XML"                        |
| **E** tentamos importar o XML vazio                                 |
| **ENTÃO** o sistema exibe a mensagem de erro                        |

| **Critérios de aceitação**                                          |
| :--------------------------------------------------------------     |
| A sistema não deve aceitar XML vazi.                                |
| [Video](https://drive.google.com/file/d/15_13DcOKZLeJeLkUVZ3PHwwwAlzNMKII/view?usp=drive_link)                                                       |

---