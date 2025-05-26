## **1. Propósito**

O objetivo deste sistema é informatizar os processos de agendamento, gerenciamento de pacientes, controle de prontuários eletrônicos, e organização financeira de uma clínica odontológica. O sistema visa melhorar a produtividade dos profissionais e a eficiência do atendimento ao paciente.

---

## **2. Escopo**

O sistema permitirá:

- Agendamento de consultas baseado na disponibilidade de salas.
- Gerenciamento de pacientes (criação, edição de informações).
- Controle de prontuário eletrônico, incluindo anexos e assinatura digital.
- Envio de lembretes automáticos via WhatsApp.
- Registro de informações financeiras associadas a consultas, sem realizar processamento de pagamento.
- Controle do status das consultas (confirmada, realizada, cancelada, remarcada).

---

## **3. Visão Geral dos Atores**

### **3.1 Secretária**

- Visualizar e gerenciar a agenda de todos os dentistas, organizada por salas.
- Marcar, alterar, cancelar e remarcar consultas.
- Cadastrar novos pacientes e editar informações dos pacientes existentes.
- Visualizar e inserir informações financeiras na consulta (valor e forma de pagamento).
- Anexar documentos no prontuário do paciente.

### **3.2 Dentista**

- Visualizar apenas sua própria agenda.
- Consultar e editar o prontuário eletrônico dos seus próprios pacientes.
- Anexar arquivos clínicos ao prontuário (exames, radiografias, fotos).
- Realizar a assinatura eletrônica do prontuário por meio de um dispositivo compatível (tablet ou smartphone).

---

## **4. Requisitos Funcionais Principais**

- **Agenda Unificada:** A secretária visualiza a agenda geral das salas.
- **Agenda Individual:** Cada dentista visualiza apenas suas consultas.
- **Gestão de Pacientes:** CRUD completo de pacientes (Create, Read, Update, Delete).
- **Controle de Consultas:** Cada consulta possui um status: Confirmada, Realizada, Cancelada ou Remarcada.
- **Anexos no Prontuário:** Possibilidade de upload de documentos e imagens no prontuário do paciente.
- **Lembretes Automatizados:** Sistema envia lembrete de consulta via WhatsApp.
- **Assinatura Eletrônica:** Dentista assina o prontuário eletrônico via dispositivo touch.
- **Financeiro Integrado ao Agendamento:** Registro de informações financeiras no agendamento, sem realizar cobrança.

---

## **5. Requisitos Não Funcionais**

- **Escalabilidade:** Suporte a N dentistas e N salas sem limitação técnica fixa.
- **Segurança:** Controle rigoroso de acesso baseado em perfis (secretária e dentistas).
- **Privacidade:** Conformidade com a LGPD, proteção de dados de saúde e pessoais dos pacientes.
- **Disponibilidade:** Sistema disponível em horário comercial (mínimo), com backup periódico.
- **Compatibilidade:** Sistema web responsivo para desktop e tablets.
- **Integração WhatsApp:** Usar API oficial para envio de lembretes, considerando custos e limites da plataforma.

---

## **6. Restrições**

- O sistema atenderá apenas uma única unidade da clínica (não multi-clínica).
- O sistema apenas registra informações financeiras; não realiza cobranças ou integrações bancárias.
- Anexos no prontuário devem respeitar limites de tamanho e tipos de arquivo compatíveis (ex: PDF, JPG, PNG).

---

## **7. Fluxo Principal de Uso**

1. Secretária cadastra paciente (se ainda não existir).
2. Secretária agenda consulta vinculando paciente, dentista e sala disponível.
3. Secretária preenche informações financeiras previstas (valor, forma de pagamento).
4. Sistema registra o status da consulta como **Confirmada**.
5. Sistema envia lembrete automático via WhatsApp próximo da data e horário da consulta.
6. Dentista realiza atendimento, preenche e anexa documentos no prontuário eletrônico.
7. Dentista assina o prontuário digitalmente.
8. Secretária ou dentista atualizam o status da consulta para **Realizada**, **Remarcada** ou **Cancelada** conforme o caso.

---

## **8. Visão de Produto**

O produto final será um sistema amigável, eficiente e seguro para o gerenciamento de uma clínica odontológica, voltado a agilizar processos internos, garantir qualidade de atendimento ao paciente, aumentar a organização e prover uma visão financeira simplificada para gestão clínica e pessoal dos dentistas.