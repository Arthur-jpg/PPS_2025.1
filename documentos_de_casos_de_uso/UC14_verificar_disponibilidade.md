# Caso de Uso: Verificar disponibilidade

**Atores:** Secretaria (indiretamente)

**Descrição:**
Permite ao sistema verificar automaticamente a disponibilidade de horários para agendamento de consultas, considerando os horários já ocupados pelos dentistas e salas.

**Fluxo Principal:**
1. Durante o processo de marcação de consulta, o sistema recebe os parâmetros de data, horário e dentista desejados.
2. O sistema consulta a agenda do dentista selecionado.
3. O sistema verifica se não há conflitos de horário na data e horário informados.
4. O sistema retorna a confirmação de disponibilidade ou lista de conflitos.

**Fluxos Alternativos:**
- Caso o horário não esteja disponível, o sistema pode sugerir horários alternativos próximos.
- Se o dentista não estiver disponível, o sistema pode sugerir outros profissionais.

**Pré-condições:**
- O dentista deve estar cadastrado no sistema.
- A data e horário desejados devem ser informados.

**Pós-condições:**
- Disponibilidade verificada e confirmada ou rejeitada.
