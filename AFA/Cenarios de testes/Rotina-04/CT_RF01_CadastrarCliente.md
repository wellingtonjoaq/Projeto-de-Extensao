Link da Rotina 04: [Video](https://drive.google.com/drive/folders/1UjRtMvVODyy10u9VWJ6EdowC7R3ApxSQ?usp=sharing)

## Cenário 06: Gestão de Clientes

### Caso de Teste 01: Cadastrar novos clientes (PF e PJ).

| ID       | Descrição                                                            |
| :------- | :------------------------------------------------------------------- |
| C06-CT01 | O sistema deve permitir cadastrar novos clientes, sendo Pessoa Física e Pessoa Jurídica. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve ter acesso ao painel de Cadastro de Clientes.  |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acesse ao painel “Cadastro de Clientes”      |
| **E** clique no botão “Novo”                                       |
| **E** preenche todas as informações necessarias (PF ou PJ)             |
| **QUANDO** clicar no botão “Salvar”                               |
| **ENTÃO** o cliente deve ser cadastrado com sucesso               |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O cliente deve aparecer na lista.                  |
| [Video](https://drive.google.com/file/d/1_LQpIx4U7hkzw6wEKGu4dGRbrEvT8MRd/view?usp=sharing) |

---

### Caso de Teste 02: Tentar cadastrar cliente com campos obrigatórios vazios.

| ID       | Descrição                                                                       |
| :------- | :-------------------------------------------------------------------------------|
| C06-CT02 | Sistema não deve permitir o cadastro de cliente sem preencher campos obrigatórios.   |  

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Usuário com acesso ao painel de cadastro.                        |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário clique em “Novo”                           |
| **E** deixa um ou mais campos obrigatórios sem preencher              |
| **QUANDO** clicar em “Salvar”                                     |
| **ENTÃO** o sistema deve exibir mensagens de erro indicando os campos que não foram preenchidos |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema NÃO deve salvar o cliente. |
| [Video](https://drive.google.com/file/d/1qCRA9oSv6L6W_LD6QQzrZKEJZDzZyOgx/view?usp=sharing) |

---

### Caso de Teste 03: Habilitar limite de crédito para cliente.

| ID       | Descrição                                                      |
| :------- | :------------------------------------------------------------- |
| C06-CT03 | O sistema deve permitir configurar limite de crédito para clientes. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Cliente cadastrado no sistema.                                |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário abra a tela “Cadastro de Clientes”        |
| **E** clique em “Novo” ou em “Alterar”  |
| **E** acesse a aba “Dados Financeiros”                            |
| **E** digite um limite de crédito e condição                    |
| **QUANDO** clicar em “Salvar”                                     |
| **ENTÃO** o limite deve ser registrado               |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O limite de crédito deve aparecer na aba Dados Financeiros depois de salvar.  |
| [Video](https://drive.google.com/file/d/1iPi1N6zWeZrM84HypwNxexc1iRIw6NPL/view?usp=sharing) |

---

### Caso de Teste 04: Informar limite de crédito inválido.

| ID       | Descrição                                                      |
| :------- | :------------------------------------------------------------- |
| C06-CT04 | Sistema não deve permitir salvar limite de crédito com valores inválidos. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Cliente cadastrado no sistema.                                |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acesse a aba “Dados Financeiros”          |
| **E** informe um valor de limite negativo ou não numérico          |
| **QUANDO** clicar em “Salvar”                                     |
| **ENTÃO** o sistema deve exibir erro e impedir o salvamento       |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Deve existir mensagem orientando o usuário.               |
| [Video](https://drive.google.com/file/d/1gDSJXA-A6FnT9uSX_JfANQCsN1qmDzD7/view?usp=sharing) |

---

### Caso de Teste 05: Adicionar dependentes a clientes.

| ID       | Descrição                                                      |
| :------- | :------------------------------------------------------------- |
| C06-CT05 | Sistema deve permitir adicionar dependentes ao cliente.        |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Cliente cadastrado no sistema.                                |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário selecione o cliente e clique em “Dependentes”   |
| **E** clica no botão “Novo”                                       |
| **E** busque os dados do dependente                             |
| **QUANDO** clicar em “Salvar”                                     |
| **ENTÃO** o dependente deve ser exibido na lista de dependentes do cliente  |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Dependente deve aparecer corretamente vinculado ao cliente.     |
| [Video](https://drive.google.com/file/d/1mwjB64xI4hu4-FnJiQZb1MNQCiB-wvv0/view?usp=sharing) |

---

### Caso de Teste 06: Registrar vendas para os clientes.

| ID       | Descrição                                                      |
| :------- | :------------------------------------------------------------- |
| C06-CT06 | Sistema deve permitir registrar vendas para clientes           |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Clientes e produtos cadastrado no sistema.                                |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuároio acesse o painel “Venda”                     |
| **E** clique no botão “Novo”                                       |
| **E** informe o cliente                                           |
| **E** adiciona um produto                                         |
| **QUANDO** clicar em “Salvar”                                     |
| **ENTÃO** a venda deve ser registrada corretamente                |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| A venda deve ser registrada corretamente.                       |
| [Video](https://drive.google.com/file/d/167DXIcrrSbsWmjANV_yNSEQh8HCX9ymI/view?usp=sharing) |

---

### Caso de Teste 07: Venda dentro do limite de crédito.

| ID       | Descrição                                                      |
| :------- | :------------------------------------------------------------- |
| C06-CT07 | Sistema deve permitir venda dentro do limite de crédito        |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Clientes e produtos cadastrado no sistema.                                |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o cliente possui limite de crédito                   |
| **E** a soma da compra dentro do limite                           |
| **QUANDO** Clicar em finalizar a venda                            |
| **ENTÃO** a venda deve ser registrada corretamente                |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| A venda deve ser registrada corretamente                        |
| [Video](https://drive.google.com/file/d/1DdTj6Fl6ZQPG0DSb8LfR_bm0zwItEdQs/view?usp=sharing) |

---

### Caso de Teste 08: Atualizar limite de crédito.

| ID       | Descrição                                                      |
| :------- | :------------------------------------------------------------- |
| C06-CT08 | SSistema deve permitir alterar o limite de crédito de um cliente  |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Cliente existente com limite cadastrado.                      |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o operador acessa o cadastro do cliente              |
| **E** clica em “Alterar”                                          |
| **E** altera o limite de crédito                                  |
| **QUANDO** Caltera o limite de crédito                            |
| **ENTÃO** o novo limite deve ser atualizado                       |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |  
| O valor atualizado deve ser exibido corretamente na aba financeira.  |                                               
| [Video](https://drive.google.com/file/d/1s-scWfJvUeqMdQru_dEwW-hY_yqXHVdv/view?usp=sharing) |

---

### Caso de Teste 09: Editar cliente.

| ID       | Descrição                                                            |
| :------- | :------------------------------------------------------------------- |
| C09-CT09 | O sistema deve permitir a edição de clientes                         |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado e ter acesso ao módulo cadastro de transportadoras. |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o operador acessa o menu “Cadastro de cliente"       |
| **E** clica no botão “Editar”                                     |
| **E** alterar o nome do cliente                                   |
| **QUANDO** clicar no botão “Salvar”                               |
| **ENTÃO** os dados do cliente deve ser alterado com sucesso       |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O cliente deve aparecer com os dados alterados.                 |
| [Video](https://drive.google.com/file/d/1eEaS8WnXN9_vYq87YFwTKp2i8TIIcoim/view?usp=sharing) |

---

### Caso de Teste 10: Excluir cliente

| ID       | Descrição                                                                 |
| :------- | :-------------------------------------------------------------------      |
| C09-CT10 | O sistema deve permitir a exclusão clientes                               |

| **Pré-condições**                                                                    |
| :------------------------------------------------------------                        |
| O usuário deve estar logado e ter acesso ao módulo cadastro de clientes.             |

| **Passos**                                                                           |
| :----------------------------------------------------------------                    |
| **DADO** que o operador esta na tela de "Cadastro de Clientes"                       |
| **QUANDO** clico no botão com icone de “Lupa”                                        |  
| **ENTÃO** o sistema abre a tela de "Pesquisa Rapida"                                 |
| **QUANDO** clico no botão "Pesquisar"                                                |  
| **ENTÃO** o sistema lista todos registros na tela                                    |
| **E** escolho um dos registros                                                       |
| **QUANDO** clico em "Ok"                                                             |  
| **ENTÃO** o sistema volta a tela de "Cadastro de Clientes" com os dados do registro selecionada                                                                            |
| **QUANDO** clico em "Excluir"                                                        |  
| **ENTÃO** o sistema exibe uma mensagem de confirmação                                |
| **QUANDO** clico em "Sim"                                                            |  
| **ENTÃO** o sistema fecha a mensagem com os dados de outro registro na tela                                                                                   |
| **QUANDO** clico no botão com icone de “Lupa”                                        |  
| **ENTÃO** o sistema abre a tela de "Pesquisa Rapida"                                 |
| **QUANDO** clico no botão "Pesquisar"                                                |  
| **ENTÃO** o sistema lista todos registros na tela menos oque foi excluido            |

| **Critérios de aceitação**                                                           |
| :--------------------------------------------------------------                      |
| O cliente deve ser deletado com sucesso                                              |
| [Video](https://drive.google.com/file/d/17LzaDvc7DzyAalcPqvS2GDrC9cxhuNws/view?usp=drive_link)                                                                        |   
