# Caso de Uso: Cadastrar paciente

**Atores:** Secretaria

**Descrição:**
Permite à secretária cadastrar novos pacientes no sistema, registrando informações pessoais, dados de contato e outras informações relevantes para atendimento odontológico.

**Fluxo Principal:**
1. A secretária acessa a opção de cadastro de paciente.
2. Insere os dados pessoais do paciente (nome, CPF, data de nascimento, gênero).
3. Insere informações de contato (telefone, email, endereço).
4. Registra informações complementares.
5. O sistema valida o CPF do paciente.
6. O sistema salva o cadastro do novo paciente.

**Fluxos Alternativos:**
- Caso o CPF seja inválido, o sistema exibe mensagem de erro e solicita correção.
- Caso o CPF já esteja cadastrado, o sistema alerta que o paciente já existe.

**Pré-condições:**
- Secretária deve estar autenticada no sistema.

**Pós-condições:**
- Novo paciente cadastrado no sistema e disponível para agendamento de consultas.
