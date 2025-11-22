Link da Rotina 03: https://drive.google.com/drive/folders/10MVFuvdmUGwjxlvX59j59lxgwZb_3IMJ?usp=sharing

## Cenário 0: Compra com Fornecedores

### Caso de Teste 01: Cadastrar novo fornecedor com informações válidas

| ID       | Descrição                                                              |
| :------- | :---------------------------------------------------------------------- |
| C0-CT01 | O sistema precisa possibilitar o cadastro de um novo fornecedor utilizando informações válidas. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário precisa estar logado e ter permissão para acessar o módulo "Cadastro de Fornecedores". |

| **Passos**                                                       |
| :--------------------------------------------------------------- |
| **DADO** que o usuário acessa o painel principal                   |
| **E** clica no segundo ícone “Cadastro de Fornecedores”                  |
| **E** clica no botão “Novo”                                      |
| **E** preenche os campos obrigatórios do fornecedor              |
| **QUANDO** clicar no botão “Salvar”                              |
| **ENTÃO** o fornecedor deve ser cadastrado com sucesso e exibido na lista.   |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O fornecedor deve ser cadastrado com sucesso                   |
| [Video](https://drive.google.com/file/d/1GWtVyqvuUGt2kSyC72BMiwmcle57G1zn/view?usp=sharing) |

---

### Caso de Teste 02: Tentar cadastrar fornecedor com campos obrigatórios vazios

| ID       | Descrição                                                                     |
| :------- | :------------------------------------------------------------------------------ |
| C05-CT02 | O sistema não deve permitir o registro e mostrar mensagens de erro quando campos obrigatórios não forem preenchidos. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Pré-condições
| O usuário deve estar na tela de Cadastro de Fornecedores.     |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário clica no botão “Novo” na tela de cadastro de fonecedor  |
| **E** não preenche os campos obrigatórios                         |
| **QUANDO** clicar em “Salvar”                                     |
| **ENTÃO** mensagens de erro devem ser exibidas nos campos obrigatórios. |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema não deve permitir finalizar o cadastro.               |
| [Video](https://drive.google.com/file/d/1NBVnMopPtZ6PaVS1CmzSfqariROtZsyd/view?usp=sharing) |

---

### Caso de Teste 03: Gerar pedido de compra 

| ID       | Descrição                                                        |
| :------- | :---------------------------------------------------------------- |
| C05-CT03 | O sistema deve permitir gerar um pedido de compra com 10 itens válidos. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Um fornecedor válido deve estar cadastrado.                 |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acesse o painel “Compra”                    |
| **E** clica no botão “Novo”                                       |
| **E** informa um fornecedor        |
| **E** clica em “Salvar”                                           |
| **E** clica no botão “Novo” para entrada de produtos              |
| **E** adiciona o primeiro produto |
| **E** clica em “Salvar”                                           |
| **QUANDO** clicar em “Finalizar”                                  |
| **ENTÃO** o pedido de compra deve ser gerado com sucesso.        |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O pedido deve conter itens cadastrados.                         |
| [Video](https://drive.google.com/file/d/1NOT9yYBBDC0zNbr2b0bVz3Aru08-rYP1/view?usp=sharing) |

---

### Caso de Teste 04: Tentar gerar compra sem selecionar fornecedor.

| ID       | Descrição                                                        |
| :------- | :---------------------------------------------------------------- |
| C05-CT04 | O sistema não deve permitir gerar um pedido de compra sem informar um fornecedor. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário está na tela de Compra.                             |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acesse a tela de “Compra”                    |
| **E** que o usuário acesse Compra e clica em “Novo”              |
| **E** NÃO informa o fornecedor                                    |
| **QUANDO** tentar clicar em “Salvar”                              |
| **ENTÃO** o sistema deve exibir mensagem exigindo seleção de fornecedor.  |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| A compra não deve ser criada sem fornecedor.                    |
| [Video](https://drive.google.com/file/d/1OyAbpTug0GKI9oqPeig9Ts8v0axc78gI/view?usp=sharing) |

---

### Caso de Teste 05: Simular parcelamento em 5 vezes e pagar parcelas.

| ID       | Descrição                                                        |
| :------- | :---------------------------------------------------------------- |
| C05-CT05 | O sistema deve permitir parcelar em 5 vezes e efetuar pagamento total da 1ª e parcial da 2ª. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Compra finalizada e registrada no sistema.                    |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o operador acessa o menu “Compra”                    |
| **E** clica no botão “Novo”                                       |
| **E** informa o fornecedor (buscando por código ou nome)          |
| **E** clica em “Salvar”                                           |
| **E** clica no ícone “Novo” para entrada de produtos              |
| **E** adiciona o primeiro produto informando código ou pesquisando por nome |
| **E** clica em “Salvar”                                           |
| **E** na tela compra clicar em "Salvar"                           |
| **E** seleciona condição de compra Prazo                          |
| **QUANDO** clicar em “Salvar”                                     |
| **ENTÃO** o sistema deve abrir a tela Contas a Pagar              |
| **E** o operador informa 5 parcelas                               |
| **E** clica em “Salvar”                                           |
| **E** efetua pagamento total da 1ª parcela                        |
| **E** efetua pagamento parcial da 2ª parcela                      |
| **QUANDO** confirmar o pagamento parcial                          |
| **ENTÃO** deve aparecer a mensagem perguntando se deseja quitar parcialmente |
| **E** o operador seleciona “Sim”                                  |
| **ENTÃO** o sistema deve registrar parcelas pagas, parcial e não pagas. |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| A lista de parcelas deve exibir: pago,  parcial e não pago.     |
| [Video](https://drive.google.com/file/d/1B4qP2WBkSuvo6n5XtAZMTFkV2gYEqoev/view?usp=sharing) |

---

### Caso de Teste 06: Fechamento de caixa.

| ID       | Descrição                                                        |
| :------- | :---------------------------------------------------------------- |
| C05-CT06 | O sistema deve permitir realizar o fechamento de caixa corretamente. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Deve existir movimentação financeira registrada.              |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o operador acessa o menu “Livro de Caixa”            |
| **E** valida os itens da compra                                   |
| **QUANDO** clicar em “Fechar Caixa”                               |
| **E** confirmar em “Fechar caixa”                                 |
| **E** clica em “Salvar”                                           |
| **ENTÃO** o caixa deve ser fechado corretamente.                  |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema deve registrar o fechamento e permitir saída da tela. |
| [Video](https://drive.google.com/file/d/1b-iwLdDyjsUOo0O9ShM6pTH7IN076_YW/view?usp=drive_link) |

---

### Caso de Teste 07: Editar fornecedor.

| ID       | Descrição                                                            |
| :------- | :------------------------------------------------------------------- |
| C09-CT07 | O sistema deve permitir a edição de fornecedores                     |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado e ter acesso ao módulo cadastro de fornecedores.    |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o operador acessa o menu “Cadastro de fornecedores"  |
| **E** clica no botão “Editar”                                     |
| **E** alterar o nome do fornecedor                                |
| **QUANDO** clicar no botão “Salvar”                               |
| **ENTÃO** os dados do fornecedor deve ser alterado com sucesso    |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O fornecedor deve aparecer com os dados alterados.              |
| [Video](https://drive.google.com/file/d/1znejuTZTUNUgN9dLXzLEoWT3L0vKecLJ/view?usp=sharing) |

---

### Caso de Teste 08: Excluir fornecedor

| ID       | Descrição                                                            |
| :------- | :------------------------------------------------------------------- |
| C09-CT08 | O sistema deve permitir a exclusão cd fornecedores                   |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado e ter acesso ao módulo cadastro de fornecedores.    |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o operador acessa o menu “gestão de fornecedores”    |
| **QUANDO** clicar no botão “excluir”                              |
| **E** clicar pra confirmar a exclusão                             |
| **ENTÃO** o fornecedor deve ser deletado com sucesso              |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| o fornecedor deve ser deletado com sucesso                      |
| [Video](https://drive.google.com/file/d/1DHDaZALhQLEqQHkaffDm_blK8x8np6NN/view?usp=sharing) |
