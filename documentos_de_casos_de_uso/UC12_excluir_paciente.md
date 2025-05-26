# Caso de Uso: Excluir paciente

**Atores:** Secretaria

**Descrição:**
Permite à secretária excluir o cadastro de um paciente do sistema, removendo todas as informações associadas, quando necessário.

**Fluxo Principal:**
1. A secretária acessa o cadastro do paciente.
2. Solicita a exclusão do paciente.
3. O sistema solicita confirmação da ação.
4. Após confirmação, o sistema remove o paciente e seus dados.

**Fluxos Alternativos:**
- Caso o paciente possua consultas futuras, o sistema alerta sobre a necessidade de remanejamento.

**Pré-condições:**
- O paciente deve estar cadastrado no sistema.

**Pós-condições:**
- Cadastro do paciente removido do sistema.
