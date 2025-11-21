# Relatório de Bugs

**Software:** OrangeHRM

**QA responsável:** Miguel Luis

**Data:** 12.05.25

---

### 🐞 **Bug 01: Ícone de visualizar senha desaparece ao clicar fora do campo**

| **ID**     | **Descrição**                                                                                                                                             |
| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BUG-001    | O ícone de “ver senha” não está sendo apresentado, impedindo o usuário de visualizar a senha digitada. |

| **Severidade do Bug** | **Prioridade de Correção** | **Status** |
| :-------------------: | :------------------------: | :--------: |
|         Média         |            Alta            |   Aberto   |

| **Passo a passo para simular o bug**                           |
| -------------------------------------------------------------- |
| 1. Acessar a página de login                                   |
| 2. Digitar o login no campo apropriado                         |
| 3. Digitar a senha no campo apropriado                         |
| 4. Ícone de "ver senha" não está disponível                             |

|                        **Comportamento Esperado**                       |                        **Comportamento Obtido**                        |
| :---------------------------------------------------------------------: | :--------------------------------------------------------------------: |
| O ícone de "ver senha" deve estar sempre visível, para ver a senha digitada | O ícone / botão de revelar senha digitada não está sendo apresentado! |

| **Ambiente**              |
| ------------------------  |
| Ambiente de homologação.  |
| Desktop com Windows 11.   |
|  Google Chrome v.142.0.74 |
| OrangeHRM Demo            |

| **Funcionalidade Afetada** |        **Caso de Teste Relacionado**       |
| :------------------------: | :----------------------------------------: |
| Login / Criação de usuário | C01-CT01: Login com e-mail e senha válidos |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo](https://jam.dev/c/9b67c5d3-e0df-467d-b477-cc61e39b7e03) |

---

#### Bug 02: Página de login atualiza ao ocorrer erro de autenticação

| **ID**     | **Descrição**                                                                                                          |
| ---------- | ------------------------------------------------------------------------------------------------------------------------ |
| BUG-002    | Ao inserir credenciais incorretas no login, a página é atualizada, o que prejudica a experiência do usuário (UX/UI).    |

| **Severidade do Bug** | **Prioridade de Correção** | **Status** |
| :-------------------: | :------------------------: | :--------: |
|         Baixa         |           Média            |   Aberto   |

| **Passo a passo para simular o bug**                        |
| ----------------------------------------------------------- |
| 1. Acessar a página de login                                |
| 2. Inserir um nome de usuário ou senha inválidos            |
| 3. Clicar no botão "Login"                                  |

|                     **Comportamento Esperado**                      |                   **Comportamento Obtido**                   |
| :-----------------------------------------------------------------: | :-----------------------------------------------------------: |
| Exibir mensagem de erro sem atualizar a página                     | A página é atualizada e apenas então exibe a mensagem de erro, limpando os campos. |

| **Ambiente**              |
| ------------------------  |
| Ambiente de homologação.  |
| Desktop com Windows 11.   |
|  Google Chrome v.142.0.74 |
| OrangeHRM Demo            |

| **Funcionalidade Afetada** |         **Caso de Teste Relacionado**         |
| :------------------------: | :-------------------------------------------: |
|           Login            | C01-CT02: Login com credenciais inválidas     |

|              **Evidência(s)**              |
| :----------------------------------------: |
| [Vídeo](https://jam.dev/c/66fc8986-d80a-4fe5-bd57-c5655418c985) |

---

#### Bug 03: Não há mensagem clara de sucesso ou falha no login

| **ID**     | **Descrição**                                                                                                     |
| ---------- | ------------------------------------------------------------------------------------------------------------------- |
| BUG-003    | O sistema não exibe mensagens de sucesso ou erro de forma clara após login, apenas redireciona ou atualiza a página. |

| **Severidade do Bug** | **Prioridade de Correção** | **Status** |
| :-------------------: | :------------------------: | :--------: |
|         Média          |           Média            |   Aberto   |

| **Passo a passo para simular o bug**              |
| ------------------------------------------------- |
| 1. Acessar a página de login                      |
| 2. Inserir credenciais válidas                    |
| 3. Clicar em "Login"                              |

|                   **Comportamento Esperado**                   |                 **Comportamento Obtido**                  |
| :-------------------------------------------------------------: | :--------------------------------------------------------: |
| Mensagem como "Login realizado com sucesso" deve ser exibida   | Usuário é redirecionado diretamente sem mensagem alguma    |

| **Ambiente**              |
| ------------------------  |
| Ambiente de homologação.  |
| Desktop com Windows 11.   |
|  Google Chrome v.142.0.74 |
| OrangeHRM Demo            |

| **Funcionalidade Afetada** |         **Caso de Teste Relacionado**         |
| :------------------------: | :-------------------------------------------: |
|           Login            | C01-CT01: Login com e-mail e senha válidos    |

|               **Evidência(s)**               |
| :------------------------------------------: |
| [Vídeo](https://jam.dev/c/7330a271-dce8-42d4-b51d-a83d6a54e345)  |

