# Cenário 09: Consulta de colaboradores no módulo Diretório

## Caso de Teste 01: Buscar colaborador por nome com sucesso

| ID       | Descrição                                                               |
| :------- | :---------------------------------------------------------------------- |
| C09-CT01 | O sistema deve retornar corretamente o colaborador pesquisado pelo nome. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado no sistema.                       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Directory\"              |
| **E** insere o nome de um colaborador existente no campo de busca |
| **QUANDO** clicar em \"Search\"                                 |
| **ENTÃO** o sistema deve exibir o colaborador correspondente à busca |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O nome, cargo e localização do colaborador devem ser exibidos corretamente. |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo]([C09-CT01] (https://jam.dev/c/a8467777-ef15-456b-8c92-27f0e66e7f1e)) |

---

### Caso de Teste 02: Buscar colaborador inexistente

| ID       | Descrição                                                                   |
| :------- | :-------------------------------------------------------------------------- |
| C09-CT02 | O sistema deve exibir uma mensagem apropriada quando nenhum colaborador for encontrado. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado no sistema.                       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Directory\"              |
| **E** digita um nome que não corresponde a nenhum colaborador    |
| **QUANDO** clicar em \"Search\"                                 |
| **ENTÃO** uma mensagem como \"No Records Found\" deve ser exibida |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema deve exibir claramente que não há registros encontrados. |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo]([C09-CT02] (https://jam.dev/c/f4a5e683-48fd-41f4-9c7d-f7fc1939b5fe)) |

---

### Caso de Teste 03: Aplicar filtro por cargo (Job Title)

| ID       | Descrição                                                                |
| :------- | :------------------------------------------------------------------------ |
| C09-CT03 | O sistema deve permitir a filtragem de colaboradores por cargo.           |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado e o sistema deve conter dados de funcionários. |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Directory\"              |
| **E** seleciona um cargo no campo \"Job Title\"                 |
| **QUANDO** clicar em \"Search\"                                 |
| **ENTÃO** apenas os colaboradores com o cargo selecionado devem ser listados |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O filtro deve funcionar corretamente e retornar apenas resultados válidos. |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo]([C09-CT03] (https://jam.dev/c/e2239fa4-5ad4-46a9-938d-d7d8d97ce7e4)) |

---
