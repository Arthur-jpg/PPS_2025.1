# Casos de Uso - Sistema de Clínica Odontológica

## UC1: Efetuar Login

**Atores:** Secretaria, Dentista

**Descrição:**
Permite que usuários autorizados (secretária e dentistas) acessem o sistema da clínica odontológica por meio de autenticação, garantindo o controle de acesso conforme o perfil do usuário.

**Fluxo Principal:**
1.  O usuário acessa a tela de login do sistema.
2.  Informa suas credenciais (usuário e senha).
3.  O sistema valida as credenciais.
4.  O sistema libera o acesso conforme o perfil (secretária ou dentista).

**Fluxos Alternativos:**
-   Se as credenciais estiverem incorretas, o sistema exibe mensagem de erro e solicita nova tentativa.

**Pré-condições:**
-   O usuário deve estar cadastrado no sistema.

**Pós-condições:**
-   O usuário tem acesso às funcionalidades permitidas pelo seu perfil.

---

## UC2: Visualizar agenda unificada

**Atores:** Secretaria, Dentista

**Descrição:**
Permite à secretária e aos dentistas visualizar a agenda completa de consultas da clínica, incluindo todos os dentistas e horários disponíveis, para melhor gerenciamento e organização.

**Fluxo Principal:**
1.  O usuário acessa a opção de agenda unificada.
2.  O sistema exibe todas as consultas agendadas, horários livres e ocupados de todos os dentistas.

**Fluxos Alternativos:**
-   Caso não haja consultas agendadas, o sistema exibe a agenda vazia.

**Pré-condições:**
-   O usuário deve estar autenticado no sistema.

**Pós-condições:**
-   O usuário visualiza a agenda unificada da clínica.

---

## UC3: Visualizar agenda individual

**Atores:** Dentista

**Descrição:**
Permite ao dentista visualizar apenas sua própria agenda de consultas, com horários disponíveis e ocupados, facilitando o gerenciamento de seus atendimentos.

**Fluxo Principal:**
1.  O dentista acessa a opção de agenda individual.
2.  O sistema exibe as consultas e horários referentes ao dentista logado.

**Fluxos Alternativos:**
-   Caso não haja consultas agendadas, o sistema exibe a agenda vazia.

**Pré-condições:**
-   O dentista deve estar autenticado no sistema.

**Pós-condições:**
-   O dentista visualiza sua agenda individual.

---

## UC4: Marcar consulta

**Atores:** Secretaria

**Descrição:**
Permite à secretária agendar consultas para pacientes, considerando a disponibilidade de dentistas e salas, registrando informações relevantes para o atendimento.

**Fluxo Principal:**
1.  A secretária acessa a opção de marcação de consulta.
2.  Informa os dados do paciente, dentista, data e horário desejados.
3.  O sistema verifica a disponibilidade e agenda a consulta.
4.  O sistema confirma o agendamento para a secretária.

**Fluxos Alternativos:**
-   Caso o horário não esteja disponível, o sistema sugere outros horários.

**Pré-condições:**
-   O paciente e o dentista devem estar cadastrados no sistema.

**Pós-condições:**
-   Consulta agendada no sistema.

---

## UC5: Confirmar horário da consulta

**Atores:** Dentista

**Descrição:**
Permite ao dentista confirmar o horário de uma consulta previamente agendada, garantindo que o paciente será atendido no horário correto.

**Fluxo Principal:**
1.  O dentista acessa sua agenda de consultas.
2.  Seleciona a consulta a ser confirmada.
3.  O sistema registra a confirmação do horário.

**Fluxos Alternativos:**
-   Caso o dentista não possa confirmar, pode sugerir novo horário ou cancelar.

**Pré-condições:**
-   Consulta deve estar previamente agendada.

**Pós-condições:**
-   Consulta confirmada no sistema.

---

## UC6: Atualizar dados do paciente

**Atores:** Secretaria

**Descrição:**
Permite à secretária atualizar informações cadastrais dos pacientes, como dados pessoais, contato e histórico, mantendo o cadastro sempre atualizado.

**Fluxo Principal:**
1.  A secretária acessa o cadastro do paciente.
2.  Realiza as alterações necessárias.
3.  O sistema salva as novas informações.

**Fluxos Alternativos:**
-   Caso o paciente não esteja cadastrado, o sistema solicita novo cadastro.

**Pré-condições:**
-   O paciente deve estar cadastrado no sistema.

**Pós-condições:**
-   Dados do paciente atualizados no sistema.

---

## UC7: Mudar status consulta

**Atores:** Secretaria

**Descrição:**
Permite à secretária alterar o status de uma consulta (confirmada, realizada, cancelada ou remarcada), mantendo o controle atualizado do andamento dos atendimentos.

**Fluxo Principal:**
1.  A secretária acessa a lista de consultas.
2.  Seleciona a consulta desejada.
3.  Altera o status conforme necessário.
4.  O sistema registra a alteração.

**Fluxos Alternativos:**
-   Caso a consulta não exista, o sistema exibe mensagem de erro.

**Pré-condições:**
-   Consulta deve estar cadastrada no sistema.

**Pós-condições:**
-   Status da consulta atualizado.

---

## UC8: Enviar mensagem automática de confirmação

**Atores:** Paciente, Sistema

**Descrição:**
Permite ao sistema enviar automaticamente mensagens de confirmação de consulta para os pacientes, utilizando canais como WhatsApp, para reduzir faltas e melhorar a comunicação.

**Fluxo Principal:**
1.  O sistema identifica consultas agendadas próximas.
2.  Envia mensagem automática de confirmação ao paciente.
3.  O paciente recebe a mensagem e pode confirmar ou solicitar alteração.

**Fluxos Alternativos:**
-   Caso o envio falhe, o sistema registra o erro e pode tentar novamente.

**Pré-condições:**
-   Consulta deve estar agendada e paciente cadastrado com contato válido.

**Pós-condições:**
-   Mensagem de confirmação enviada ao paciente.

---

## UC9: Consultar prontuário eletrônico

**Atores:** Secretaria, Dentista

**Descrição:**
Permite à secretária e aos dentistas consultar o prontuário eletrônico dos pacientes, visualizando informações clínicas, históricos de atendimentos e documentos anexados.

**Fluxo Principal:**
1.  O usuário acessa o prontuário do paciente.
2.  O sistema exibe as informações clínicas e documentos anexados.

**Fluxos Alternativos:**
-   Caso o paciente não possua prontuário, o sistema exibe mensagem informativa.

**Pré-condições:**
-   O paciente deve estar cadastrado no sistema.

**Pós-condições:**
-   Prontuário eletrônico consultado.

---

## UC10: Assinar prontuário

**Atores:** Dentista, Paciente

**Descrição:**
Permite ao dentista e ao paciente realizar a assinatura digital do prontuário eletrônico, garantindo a autenticidade das informações registradas no atendimento.

**Fluxo Principal:**
1.  O dentista finaliza o registro do atendimento no prontuário.
2.  O sistema solicita a assinatura digital do dentista e do paciente.
3.  Ambos realizam a assinatura em dispositivo touch.
4.  O sistema registra as assinaturas no prontuário.

**Fluxos Alternativos:**
-   Caso uma das partes não assine, o sistema registra o motivo e mantém o prontuário pendente.

**Pré-condições:**
-   Atendimento realizado e prontuário preenchido.

**Pós-condições:**
-   Prontuário assinado digitalmente.

---

## UC11: Registrar valores de consultas

**Atores:** Secretaria

**Descrição:**
Permite à secretária registrar valores previstos e formas de pagamento das consultas agendadas, apenas para controle interno, sem realizar cobranças diretas.

**Fluxo Principal:**
1.  A secretária acessa o agendamento da consulta.
2.  Informa o valor previsto e a forma de pagamento.
3.  O sistema registra as informações para controle interno.

**Fluxos Alternativos:**
-   Caso a consulta não exista, o sistema exibe mensagem de erro.

**Pré-condições:**
-   Consulta deve estar agendada.

**Pós-condições:**
-   Valores e formas de pagamento registrados para a consulta.

---

## UC12: Excluir paciente

**Atores:** Secretaria

**Descrição:**
Permite à secretária excluir o cadastro de um paciente do sistema, removendo todas as informações associadas, quando necessário.

**Fluxo Principal:**
1.  A secretária acessa o cadastro do paciente.
2.  Solicita a exclusão do paciente.
3.  O sistema solicita confirmação da ação.
4.  Após confirmação, o sistema remove o paciente e seus dados.

**Fluxos Alternativos:**
-   Caso o paciente possua consultas futuras, o sistema alerta sobre a necessidade de remanejamento.

**Pré-condições:**
-   O paciente deve estar cadastrado no sistema.

**Pós-condições:**
-   Cadastro do paciente removido do sistema.

---

## UC13: Cadastrar paciente

**Atores:** Secretaria

**Descrição:**
Permite à secretária cadastrar novos pacientes no sistema, registrando informações pessoais, dados de contato e outras informações relevantes para atendimento odontológico.

**Fluxo Principal:**
1.  A secretária acessa a opção de cadastro de paciente.
2.  Insere os dados pessoais do paciente (nome, CPF, data de nascimento, gênero).
3.  Insere informações de contato (telefone, email, endereço).
4.  Registra informações complementares.
5.  O sistema valida o CPF do paciente.
6.  O sistema salva o cadastro do novo paciente.

**Fluxos Alternativos:**
-   Caso o CPF seja inválido, o sistema exibe mensagem de erro e solicita correção.
-   Caso o CPF já esteja cadastrado, o sistema alerta que o paciente já existe.

**Pré-condições:**
-   Secretária deve estar autenticada no sistema.

**Pós-condições:**
-   Novo paciente cadastrado no sistema e disponível para agendamento de consultas.

---

## UC14: Verificar disponibilidade

**Atores:** Secretaria (indiretamente)

**Descrição:**
Permite ao sistema verificar automaticamente a disponibilidade de horários para agendamento de consultas, considerando os horários já ocupados pelos dentistas e salas.

**Fluxo Principal:**
1.  Durante o processo de marcação de consulta, o sistema recebe os parâmetros de data, horário e dentista desejados.
2.  O sistema consulta a agenda do dentista selecionado.
3.  O sistema verifica se não há conflitos de horário na data e horário informados.
4.  O sistema retorna a confirmação de disponibilidade ou lista de conflitos.

**Fluxos Alternativos:**
-   Caso o horário não esteja disponível, o sistema pode sugerir horários alternativos próximos.
-   Se o dentista não estiver disponível, o sistema pode sugerir outros profissionais.

**Pré-condições:**
-   O dentista deve estar cadastrado no sistema.
-   A data e horário desejados devem ser informados.

**Pós-condições:**
-   Disponibilidade verificada e confirmada ou rejeitada.

---

## UC15: Selecionar sala

**Atores:** Secretaria

**Descrição:**
Permite à secretária selecionar uma sala apropriada para a realização da consulta, com base na disponibilidade e características necessárias para o atendimento.

**Fluxo Principal:**
1.  Durante o processo de marcação de consulta, a secretária verifica salas disponíveis.
2.  O sistema exibe a lista de salas livres no horário selecionado.
3.  A secretária seleciona uma sala adequada para o atendimento.
4.  O sistema registra a sala como ocupada para aquele horário.

**Fluxos Alternativos:**
-   Caso não exista sala disponível no horário desejado, o sistema informa a indisponibilidade.
-   A secretária pode visualizar os recursos disponíveis em cada sala antes de selecionar.

**Pré-condições:**
-   Horário de consulta já definido.
-   Dentista já selecionado para o atendimento.

**Pós-condições:**
-   Sala reservada para a consulta.

---

## UC16: Anexar documentos

**Atores:** Secretaria, Dentista

**Descrição:**
Permite à secretária e aos dentistas anexar documentos digitais ao prontuário do paciente, como exames, radiografias, fotos clínicas e outros arquivos relevantes para o tratamento.

**Fluxo Principal:**
1.  O usuário acessa o prontuário do paciente.
2.  Seleciona a opção de anexar documentos.
3.  Escolhe o tipo de documento (radiografia, foto clínica, exame laboratorial, etc).
4.  Seleciona o arquivo a ser anexado a partir do dispositivo.
5.  Adiciona uma descrição para o documento.
6.  O sistema valida o formato e tamanho do arquivo.
7.  O sistema anexa o documento ao prontuário.

**Fluxos Alternativos:**
-   Caso o arquivo tenha formato inválido ou tamanho excessivo, o sistema exibe mensagem de erro.
-   O usuário pode cancelar o anexo a qualquer momento.
-   Possibilidade de visualizar, substituir ou excluir documentos já anexados.

**Pré-condições:**
-   O paciente deve estar cadastrado no sistema.
-   Usuário deve ter permissão para acessar o prontuário.

**Pós-condições:**
-   Documento anexado ao prontuário eletrônico.

---

## UC17: Visualizar histórico

**Atores:** Secretaria, Dentista

**Descrição:**
Permite à secretária e aos dentistas visualizar o histórico completo de atendimentos, procedimentos e evolução clínica do paciente, fornecendo uma visão cronológica dos tratamentos realizados.

**Fluxo Principal:**
1.  O usuário acessa o prontuário do paciente.
2.  Seleciona a opção de visualizar histórico.
3.  O sistema exibe todas as consultas anteriores em ordem cronológica.
4.  O usuário pode filtrar por período, dentista ou tipo de procedimento.
5.  O sistema apresenta detalhes de cada atendimento quando solicitado.

**Fluxos Alternativos:**
-   Caso o paciente não possua histórico de atendimentos, o sistema exibe mensagem informativa.
-   O usuário pode exportar o histórico para formatos como PDF, se necessário.

**Pré-condições:**
-   O paciente deve estar cadastrado no sistema.
-   Usuário deve ter permissão para acessar o prontuário.

**Pós-condições:**
-   Histórico de atendimentos visualizado.

**Pós-condições:**
-   Novo paciente cadastrado no sistema e disponível para agendamento de consultas.