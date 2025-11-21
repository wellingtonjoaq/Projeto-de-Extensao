## Cenário 01: Simular operações de 3 caixas simultâneas

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
| **QUANDO** quando clico em "Salvar"                                 |
| **ENTÃO** o caixa e aberto e é listado o registro dele              |

| **Critérios de aceitação**                                          |
| :--------------------------------------------------------------     |
|  Caixa deve estar aberto.                                           |
| [Video]([]())                                                    |

---