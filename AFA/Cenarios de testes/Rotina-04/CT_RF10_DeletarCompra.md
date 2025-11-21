## Cenário 10: Deletar Produto.

### Caso de Teste 01: Deletar produto com sucesso.

| ID       | Descrição                                                            |
| :------- | :-------------------------------------------------------             |
| C04-CT01 | O sistema deve deletar o produto com sucesso.                        |

| **Pré-condições**                                                               |
| :------------------------------------------------------------                   |
| O usuario deve buscar o produto que deseja deletar.                             |

 **Passos**                                                                       |
| :----------------------------------------------------------------               |
| **DADO** que estamos na tela de cadastro de produtos                            |
| **QUANDO** clicarmos no botão "Excluir"                                         |
| **ENTÃO** ira exibir um aviso de confirmação                                    |
| **E** clica-mos em "Sim"                                                        |
| **ENTÃO** o aviso e fechado e é listado outro produto                           |

| **Critérios de aceitação**                                                      |
| :--------------------------------------------------------------                 |
| Na tela principal deve estar listada os dados de outro produto                  |
| [Video]([https://drive.google.com/file/d/1aCpfVDrBsv8whNAYpcvhTxdy6qZaaQI8/view?usp=drive_link]())                                                                | 

---