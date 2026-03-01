# Relatório de Bugs

**Software:** OrangeHRM

**QA responsável:** Rafael Dal Forno

**Data:** 10.11.25

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

### **Bug 02: Página de login atualiza ao ocorrer erro de autenticação**

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

### **Bug 03: Não há mensagem clara de sucesso ou falha no login**

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

---

### **Bug 04: Não é possível aplicar licença de férias - "No Leave Types with Leave Balance"**

| **ID**     | **Descrição**                                                                                                                |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------ |
| BUG-004    | Ao tentar aplicar uma licença no módulo de férias, nenhuma opção de licença é exibida, impossibilitando a solicitação.        |

| **Severidade do Bug** | **Prioridade de Correção** | **Status** |
| :-------------------: | :------------------------: | :--------: |
|        Alta            |           Alta             |   Aberto   |

| **Passo a passo para simular o bug**                     |
| -------------------------------------------------------- |
| 1. Acessar o menu "Leave"                                |
| 2. Clicar em "Apply"                                     |
| 3. Verificar se aparecem tipos de licença disponíveis    |

|                      **Comportamento Esperado**                       |                        **Comportamento Obtido**                         |
| :-------------------------------------------------------------------: | :----------------------------------------------------------------------: |
| Deve-se exibir uma lista de tipos de licença com saldo disponível     | A mensagem "No Leave Types with Leave Balance" é exibida e nada é listado |

| **Ambiente**              |
| ------------------------  |
| Ambiente de homologação.  |
| Desktop com Windows 11.   |
|  Google Chrome v.142.0.74 |
| OrangeHRM Demo            |

| **Funcionalidade Afetada** |               **Caso de Teste Relacionado**               |
| :------------------------: | :-------------------------------------------------------: |
|    Férias (Leave Module)   | C04-CT01: Aplicar licença de férias com dados válidos     |

|              **Evidência(s)**              |
| :----------------------------------------: |
| [Vídeo](https://jam.dev/c/8e0605be-16b8-43d5-bb3e-f4c78034af67) |

---

### **Bug 05: Ícone de “ver senha” não é apresentado no campo do formulário de criação de funcionário**

| **ID**     | **Descrição**                                                                                                                                                  |
| ---------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BUG-005    | No formulário de criação de funcionário no módulo PIM, o ícone de "ver senha" não é apresentado no campo de senha ou confirmação de senha.             |

| **Severidade do Bug** | **Prioridade de Correção** | **Status** |
| :-------------------: | :------------------------: | :--------: |
|         Média         |           Alta             |   Aberto   |

| **Passo a passo para simular o bug**                             |
| ---------------------------------------------------------------- |
| 1. Navegar até o módulo "PIM"                                    |
| 2. Clicar em "Add Employee"                                      |
| 3. Marcar a opção "Create Login Details"                         |
| 4. Observar o campo de senha e confirmação de senha, ícone não apresentado    |

|                      **Comportamento Esperado**                      |                         **Comportamento Obtido**                          |
| :------------------------------------------------------------------: | :------------------------------------------------------------------------: |
| O ícone de "ver senha" deve permanecer visível e funcional           | O ícone não é apresentado, impedindo visualização da senha digitada |

| **Ambiente**              |
| ------------------------  |
| Ambiente de homologação.  |
| Desktop com Windows 11.   |
|  Google Chrome v.142.0.74 |
| OrangeHRM Demo            |

| **Funcionalidade Afetada** |            **Caso de Teste Relacionado**             |
| :------------------------: | :--------------------------------------------------: |
| Cadastro de funcionário    | C03-CT01: Criar novo funcionário com dados válidos   |

|               **Evidência(s)**               |
| :------------------------------------------: |
| [Vídeo](https://jam.dev/c/7c8cedf2-330b-435c-8b57-69bb564aae65) |

---
