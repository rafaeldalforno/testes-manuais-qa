## Cenário 07: Registro de ponto (Controle de Horas) pelo módulo Time.

### Caso de Teste 01: Marcar ponto (Check In) com horário válido.

| ID       | Descrição                                                                  |
| :------- | :------------------------------------------------------------------------- |
| C07-CT01 | O sistema deve permitir que o usuário registre sua entrada com sucesso.    |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado e ter acesso ao módulo "Time".    |

| **Passos**                                                            |
| :-------------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Time > Attendance > Punch In\" |
| **E** verifica que o horário atual é válido                           |
| **QUANDO** clicar em \"Punch In\"                                     |
| **ENTÃO** o registro de entrada deve ser salvo com sucesso            |

| **Critérios de aceitação**                                                |
| :------------------------------------------------------------------------ |
| O sistema deve confirmar o registro com uma mensagem e salvar o horário.  |

---