# Cenário 06: Gerenciamento de usuários no módulo Administração (Admin)

## Caso de Teste 01: Adicionar um novo usuário com dados válidos.

| ID       | Descrição                                                            |
| :------- | :------------------------------------------------------------------- |
| C06-CT01 | O sistema deve permitir o cadastro de um novo usuário com informações válidas. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado com permissões de administrador.  |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o administrador acessa o menu \"Admin\"             |
| **E** clica em \"Add\"                                           |
| **E** preenche os campos obrigatórios como \"Employee Name\", \"Username\" e \"Password\" |
| **QUANDO** clicar em \"Save\"                                    |
| **ENTÃO** o novo usuário deve ser cadastrado e listado corretamente |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O usuário cadastrado deve aparecer na lista de usuários ativos. |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo]([C06-CT01] (https://jam.dev/c/1109ed34-90db-4259-bacf-8cc38df20ccb)) |

---

### Caso de Teste 02: Tentativa de adicionar usuário com nome de usuário já existente

| ID       | Descrição                                                                       |
| :------- | :------------------------------------------------------------------------------- |
| C06-CT02 | O sistema deve impedir o cadastro de um novo usuário com nome de usuário duplicado. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Já deve existir um usuário com o mesmo nome de usuário.       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o administrador acessa o menu \"Admin\"             |
| **E** clica em \"Add\"                                           |
| **E** insere um nome de usuário que já existe                   |
| **QUANDO** clicar em \"Save\"                                    |
| **ENTÃO** uma mensagem de erro \"Already exists\" deve ser exibida |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema deve impedir o cadastro e exibir mensagem de duplicidade. |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo]([C06-CT02] (https://jam.dev/c/c4ad7855-a1ac-41ae-b340-1b412d8fb19b)) |

---

### Caso de Teste 03: Filtrar usuários por status "Enabled"

| ID       | Descrição                                                      |
| :------- | :------------------------------------------------------------- |
| C06-CT03 | O sistema deve exibir apenas usuários com status "Enabled" ao aplicar o filtro. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Deve haver usuários com diferentes status (Enabled e Disabled). |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o administrador acessa o menu \"Admin\"             |
| **E** seleciona \"Enabled\" no campo \"Status\"                 |
| **QUANDO** clicar em \"Search\"                                  |
| **ENTÃO** apenas usuários com status \"Enabled\" devem ser exibidos na lista |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| A lista deve conter apenas usuários com status "Enabled".       |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo]([C06-CT03] (https://jam.dev/c/ddf6a270-3e96-42db-9a72-b6cf47dfb135)) |

---
