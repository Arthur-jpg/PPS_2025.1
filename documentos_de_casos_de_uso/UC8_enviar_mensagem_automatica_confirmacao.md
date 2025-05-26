# Caso de Uso: Enviar mensagem automática de confirmação

**Atores:** Paciente, Sistema

**Descrição:**
Permite ao sistema enviar automaticamente mensagens de confirmação de consulta para os pacientes, utilizando canais como WhatsApp, para reduzir faltas e melhorar a comunicação.

**Fluxo Principal:**
1. O sistema identifica consultas agendadas próximas.
2. Envia mensagem automática de confirmação ao paciente.
3. O paciente recebe a mensagem e pode confirmar ou solicitar alteração.

**Fluxos Alternativos:**
- Caso o envio falhe, o sistema registra o erro e pode tentar novamente.

**Pré-condições:**
- Consulta deve estar agendada e paciente cadastrado com contato válido.

**Pós-condições:**
- Mensagem de confirmação enviada ao paciente.
