## 🧪 **Plano de Testes - OrangeHRM (Demo)**

### 📌 1. **Identificação**

* **Nome do Projeto**: OrangeHRM - Sistema de Gestão de Recursos Humanos
* **Versão Avaliada**: Demo pública
* **Ambiente de Testes**: [https://opensource-demo.orangehrmlive.com](https://opensource-demo.orangehrmlive.com)
* **Tipo de Teste**: Teste Funcional Manual
* **Data do Documento**: 10/11/2025
* **Responsável (QA)**: Rafael Dal Forno

---

### 🎯 2. **Objetivo** 

Realizar a verificação manual dos principais requisitos funcionais do sistema OrangeHRM Demo, com foco em validação dos fluxos críticos, mensagens de erro, comportamento esperado e integridade das funcionalidades disponíveis na interface web.

---

### 🧩 3. **Escopo**

**Incluído**

* Autenticação de usuário
* Dashboard inicial
* Gestão de Funcionários (PIM)
* Férias (Leave)
* Recrutamento
* Administração (Admin)
* Controle de ponto (Time)
* Diretório e relatórios

**Excluídos** 

* Testes de integração com sistemas externos (não disponível na demo)
* Testes em dispositivos móveis
* Testes de performance ou carga

---

### 🔧 4. **Ferramentas Utilizadas** 

* Navegador Google Chrome / Firefox
* Ferramentas de inspeção do navegador (DevTools)
* Google Sheets ou Excel (Registro de casos e evidências)
* Captura de tela (Snipping Tool, Lightshot ou Jam)

---

### 🧪 5. **Técnicas de Teste** 

* Particionamento de equivalência
* Análise de valor limite
* Caminho feliz (Happy Path)
* Testes negativos
* Testes exploratórios

---

### 📄 6. **Critérios de Aceitação**

* Todos os casos de teste devem passar com sucesso, conforme o resultado esperado.
* Nenhuma falha crítica deve estar presente em funcionalidades principais.
* Mensagens de erro e validação devem ser consistentes.

---

### 🚦 7. **Critérios de Saída (Exit Criteria)**

* Todos os testes do escopo foram executados.
* Falhas foram registradas, analisadas e reexecutadas se necessário.
* Documentação de evidência de sucesso e falhas está completa.

---

### ⏱️ 8. **Cronograma Estimado**

| Atividade                         | Data Início | Data Fim    |
| --------------------------------- | ----------- | ----------- |
| Planejamento de Testes            | 11/11/2025  | 11/11/2025  |
| Criação de Casos de Teste         | 11/11/2025  | 12/11/2025  |
| Execução dos Testes Manuais       | 12/11/2025  | 16/11/2025  |
| Registro e Report de Bugs         | 12/11/2025  | 18/11/2025  |
| Encerramento e Evidências         | 15/11/2025  | 20/11/2025  |

---

### 📋 8. **Módulos a serem Testados**

| Código RF   | Módulo                    | Prioridade |
| ----------- | ------------------------- | ---------- |
| RF01        | Login                     | Alta       |
| RF02        | Dashboard                 | Média      |
| RF03        | PIM - Funcionários        | Alta       |
| RF04        | Férias (Leave)            | Alta       |
| RF05        | Recrutamento              | Média      |
| RF06        | Administração (Admin)     | Alta       |
| RF07        | Controle de Ponto (Time)  | Média      |
| RF08        | Relatórios                | Média      |
| RF09        | Diretório                 | Baixa      |
| RF10        | Manutenção                | Baixa      |

---

### 📌 11. **Riscos Identificados**

| Risco                                  | Impacto | Mitigação                        |
| -------------------------------------- | ------- | -------------------------------- |



---

### 📁 12. **Entregáveis** 

* Plano de Testes (.md ou .pdf)
* Casos de Teste (.md ou planilha)
* Evidências de Execução (Prints organizados por RF)
* Registro de Bugs (se houver)
* Relatório Final de Execução