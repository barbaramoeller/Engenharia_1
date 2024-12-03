# Engenharia de Software I (20242)

## Nome dos integrantes do grupo:
1. Barbara Moeller
2. Gustavo Brunoni
3. José Gabriel Paludo
4. Júlia Hackenhaar
5. Vitor Fiametti

---

## Casos de Uso do Sistema de Reserva de Passagens Aéreas

### Caso de Uso: Realizar Reserva
| **Nome do caso de uso**   | Realizar Reserva                                                                              |
|---------------------------|-----------------------------------------------------------------------------------------------|
| **Escopo**                | Sistema de reserva de passagens aéreas                                                        |
| **Nível**                 | Objetivo do usuário                                                                           |
| **Atores Principais**     | Pessoa Física                                                                                 |
| **Stakeholders e Interesses** | **Usuário**: Reservar passagem de forma eficiente.<br>**Empresa**: Registrar reservas e garantir pagamento. |
| **Pré-condições**         | O usuário deve estar cadastrado no sistema e autenticado.                                     |
| **Pós-condições de sucesso** | Reserva confirmada e registrada no sistema.                                                |
| **Pós-condições de falha**   | Reserva não registrada; o sistema notifica o usuário sobre a falha.                         |
| **Fluxo Principal**       | 1. Usuário escolhe o voo desejado.<br>2. Confirma os dados da reserva.<br>3. Realiza o pagamento. |
| **Fluxo Alternativo**     | Caso o pagamento falhe, o sistema notifica o usuário e permite tentar novamente.              |

---

### Caso de Uso: Alterar Reserva
| **Nome do caso de uso**   | Alterar Reserva                                                                               |
|---------------------------|-----------------------------------------------------------------------------------------------|
| **Escopo**                | Sistema de reserva de passagens aéreas                                                        |
| **Nível**                 | Objetivo do usuário                                                                           |
| **Atores Principais**     | Pessoa Física                                                                                 |
| **Stakeholders e Interesses** | **Usuário**: Alterar uma reserva de forma prática.<br>**Empresa**: Gerenciar alterações de forma eficiente. |
| **Pré-condições**         | O usuário deve ter uma reserva previamente realizada e estar autenticado.                     |
| **Pós-condições de sucesso** | Reserva alterada com sucesso no sistema.                                                   |
| **Pós-condições de falha**   | Alteração não realizada; o sistema notifica o usuário sobre o problema.                     |
| **Fluxo Principal**       | 1. Usuário seleciona a reserva.<br>2. Modifica os dados desejados.<br>3. Confirma as alterações. |
| **Fluxo Alternativo**     | Caso o voo selecionado não tenha vagas disponíveis, o sistema notifica o usuário.             |

---

### Caso de Uso: Cancelar Reserva
| **Nome do caso de uso**   | Cancelar Reserva                                                                              |
|---------------------------|-----------------------------------------------------------------------------------------------|
| **Escopo**                | Sistema de reserva de passagens aéreas                                                        |
| **Nível**                 | Objetivo do usuário                                                                           |
| **Atores Principais**     | Pessoa Física                                                                                 |
| **Stakeholders e Interesses** | **Usuário**: Cancelar a reserva e, se aplicável, obter reembolso.<br>**Empresa**: Registrar o cancelamento e tratar reembolsos. |
| **Pré-condições**         | O usuário deve ter uma reserva previamente realizada e estar autenticado.                     |
| **Pós-condições de sucesso** | Reserva cancelada e registro de reembolso iniciado (se aplicável).                         |
| **Pós-condições de falha**   | Cancelamento não processado; o sistema informa o motivo ao usuário.                        |
| **Fluxo Principal**       | 1. Usuário acessa suas reservas.<br>2. Seleciona a reserva a ser cancelada.<br>3. Confirma o cancelamento. |
| **Fluxo Alternativo**     | Caso a reserva já esteja no prazo limite de cancelamento, o sistema notifica o usuário.       |

---

### Caso de Uso: Consultar Voos
| **Nome do caso de uso**   | Consultar Voos                                                                                |
|---------------------------|-----------------------------------------------------------------------------------------------|
| **Escopo**                | Sistema de reserva de passagens aéreas                                                        |
| **Nível**                 | Objetivo do usuário                                                                           |
| **Atores Principais**     | Pessoa Física ou Pessoa Jurídica                                                              |
| **Stakeholders e Interesses** | **Usuário**: Visualizar voos disponíveis.<br>**Empresa**: Oferecer informações atualizadas sobre voos. |
| **Pré-condições**         | O usuário deve estar autenticado no sistema.                                                  |
| **Pós-condições de sucesso** | Voos exibidos de acordo com os critérios fornecidos.                                        |
| **Pós-condições de falha**   | Nenhum voo disponível; o sistema informa o usuário.                                         |
| **Fluxo Principal**       | 1. Usuário seleciona os critérios de busca (origem, destino, data).<br>2. Sistema exibe os voos disponíveis. |
| **Fluxo Alternativo**     | Caso não haja voos disponíveis, o sistema notifica o usuário.                                 |

---

### Caso de Uso: Solicitar Reembolso
| **Nome do caso de uso**   | Solicitar Reembolso                                                                           |
|---------------------------|-----------------------------------------------------------------------------------------------|
| **Escopo**                | Sistema de reserva de passagens aéreas                                                        |
| **Nível**                 | Objetivo do usuário                                                                           |
| **Atores Principais**     | Pessoa Física                                                                                 |
| **Stakeholders e Interesses** | **Usuário**: Recuperar o valor de uma reserva cancelada.<br>**Empresa**: Gerenciar e processar reembolsos. |
| **Pré-condições**         | O usuário deve ter cancelado uma reserva que permita reembolso.                               |
| **Pós-condições de sucesso** | Reembolso processado pelo sistema e enviado ao banco.                                       |
| **Pós-condições de falha**   | Reembolso não processado; o sistema informa o motivo ao usuário.                            |
| **Fluxo Principal**       | 1. Usuário acessa a reserva cancelada.<br>2. Solicita o reembolso.<br>3. Sistema inicia o processo com o banco. |
| **Fluxo Alternativo**     | Caso o reembolso não seja permitido, o sistema notifica o usuário.                            |


---


### Diagrama de Casos de Uso: 

![diagramacasodeusos](https://private-user-images.githubusercontent.com/177582718/391751328-313884c5-fa6a-4d4c-89f4-ff549aad258a.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzMxODM3MjEsIm5iZiI6MTczMzE4MzQyMSwicGF0aCI6Ii8xNzc1ODI3MTgvMzkxNzUxMzI4LTMxMzg4NGM1LWZhNmEtNGQ0Yy04OWY0LWZmNTQ5YWFkMjU4YS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQxMjAyJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MTIwMlQyMzUwMjFaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT01YWI0NzNmODNlNTc5MzI4Y2NiZDU4ZGMyZWVmZTlhZDg2ZWJhMzgyZGRhNjgxYWEwMmY5NDliZDBjZGRkODc2JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.0FjAF-_iBQxWlPrq7mn22L6sVGPdJTkNK7X0UyS_Qc8)


--- 

### Modelo de Domínio:

![diagramacasodeusos](https://private-user-images.githubusercontent.com/177582718/391753683-e822ed62-cbcd-4389-97cb-e915dedb71e9.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzMxODQ0NjksIm5iZiI6MTczMzE4NDE2OSwicGF0aCI6Ii8xNzc1ODI3MTgvMzkxNzUzNjgzLWU4MjJlZDYyLWNiY2QtNDM4OS05N2NiLWU5MTVkZWRiNzFlOS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQxMjAzJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MTIwM1QwMDAyNDlaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1jMGM3ZmYzNTgwYWRmNmI2N2NhNGEzZWFhM2JjNzFjMmFkN2M5MWU3NWMxZDRlYTZhMjZjMjhhYTYxNTRiOTU1JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.PZ-shWvqy9qn5x3Gx-KltOUR1_wJa06qHTKOZVMFOnA)


---

### Diagrama de Atividades:
![diagramaatividades](https://github.com/user-attachments/assets/1a138b4d-d352-42a5-9704-693da429b149)

---

### Diagrama de Classe de Implementação:

---




