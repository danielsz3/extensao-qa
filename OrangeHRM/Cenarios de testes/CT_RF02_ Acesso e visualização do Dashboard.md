# Cenário 02: Acesso e visualização do Dashboard

## Caso de Teste 01: Acesso ao Dashboard após login bem-sucedido

| ID       | Descrição                                                        |
| :------- | :---------------------------------------------------------------- |
| C02-CT01 | Verificar a exibição correta do Dashboard após login com sucesso. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar autenticado com credenciais válidas.     |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessou o sistema com sucesso              |
| **QUANDO** for redirecionado automaticamente após o login         |
| **ENTÃO** a tela do Dashboard deve ser exibida com os atalhos e widgets principais |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema deve exibir corretamente a interface do Dashboard.     |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo]([C02-CT01] (https://jam.dev/c/e3fea2a6-f18b-4fc3-9100-1d47d093d378)) |

---

### Caso de Teste 02: Verificação da exibição dos widgets do Dashboard

| ID       | Descrição                                                 |
| :------- | :-------------------------------------------------------- |
| C02-CT02 | Os widgets padrão devem ser exibidos corretamente no Dashboard. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar na tela do Dashboard após login.         |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário está autenticado                          |
| **E** está visualizando o Dashboard                              |
| **QUANDO** a página for carregada                                |
| **ENTÃO** widgets como \"Time at Work\" e \"My Actions\" devem ser exibidos |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Todos os widgets principais devem ser visíveis e funcionais.     |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo]([C02-CT02] (https://jam.dev/c/fd13f997-dda5-4883-bad3-99ac200a8902)) |

---

### Caso de Teste 03: Acesso ao Dashboard com sessão expirada

| ID       | Descrição                                                            |
| :------- | :------------------------------------------------------------------- |
| C02-CT03 | O sistema deve redirecionar o usuário para o login se a sessão estiver expirada. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário estava logado, mas a sessão expirou.                |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessou o sistema anteriormente            |
| **E** permaneceu inativo por um longo período                    |
| **QUANDO** tentar acessar o Dashboard novamente                  |
| **ENTÃO** o sistema deve redirecioná-lo para a página de login    |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| A sessão expirada deve ser tratada corretamente com redirecionamento. |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo]([C02-CT03] (https://jam.dev/c/4ee2f3f5-4092-4b6f-b488-62a2356c7c23)) |

---
