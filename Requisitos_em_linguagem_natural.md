# Requisitos do Sistema de Gerenciamento de Clínica Odontológica

## Introdução

Este documento descreve os requisitos para o sistema de gerenciamento de uma clínica odontológica, com foco na informatização dos processos de agendamento, gerenciamento de pacientes, controle de prontuários eletrônicos e organização financeira. O sistema visa melhorar a produtividade dos profissionais e a eficiência do atendimento ao paciente.

## Requisitos Funcionais

### Gestão de Usuários
1. **Efetuar Login**: O sistema deve permitir que usuários (secretárias e dentistas) acessem o sistema através de credenciais seguras, garantindo que cada perfil tenha acesso apenas às funcionalidades pertinentes ao seu papel.

### Gestão de Pacientes
1. **Cadastrar Paciente**: A secretária deve poder cadastrar novos pacientes no sistema, incluindo informações pessoais, de contato e histórico médico relevante.

2. **Atualizar Dados do Paciente**: A secretária deve poder atualizar as informações cadastrais dos pacientes já registrados no sistema.

3. **Excluir Paciente**: A secretária deve poder remover pacientes do sistema quando necessário, seguindo normas de proteção de dados.

### Gestão de Agendamento
1. **Visualizar Agenda Unificada**: A secretária deve poder visualizar a agenda de todos os dentistas organizadas por salas, facilitando o gerenciamento global dos atendimentos.

2. **Visualizar Agenda Individual**: Os dentistas devem poder visualizar apenas sua própria agenda, com detalhes sobre seus atendimentos e pacientes.

3. **Marcar Consulta**: O sistema deve permitir à secretária o agendamento de consultas, associando paciente, dentista, sala e horário.

4. **Confirmar Horário de Consulta**: O sistema deve possibilitar a confirmação de horários de consultas agendadas.

5. **Verificar Disponibilidade de Horários**: O sistema deve permitir a verificação de horários disponíveis para agendamento de consultas.

6. **Selecionar Sala para Atendimento**: O sistema deve permitir a seleção de salas disponíveis para o atendimento.

7. **Mudar Status da Consulta**: O sistema deve permitir a alteração do status da consulta (confirmada, realizada, cancelada ou remarcada).

8. **Enviar Mensagem Automática de Confirmação**: O sistema deve enviar lembretes automáticos aos pacientes via WhatsApp em proximidade da data de consulta.

### Gestão de Prontuários
1. **Consultar Prontuário Eletrônico**: Os dentistas devem poder acessar o prontuário eletrônico dos seus pacientes para consulta de informações clínicas.

2. **Assinar Prontuário**: Os dentistas devem poder realizar a assinatura eletrônica do prontuário por meio de um dispositivo compatível.

3. **Registrar Valores das Consultas**: O sistema deve permitir o registro de informações financeiras associadas às consultas.

4. **Anexar Documentos ao Prontuário**: O sistema deve permitir anexar arquivos clínicos ao prontuário, como exames, radiografias e fotos.

5. **Visualizar Histórico de Atendimentos**: O sistema deve permitir a visualização do histórico de atendimentos dos pacientes.

## Requisitos Não Funcionais

1. **Desempenho**: O sistema deve ser rápido e responsivo, garantindo que as operações sejam executadas em tempo adequado para não prejudicar o fluxo de trabalho da clínica.

2. **Segurança**: O sistema deve implementar controles rigorosos de acesso baseados em perfis, protegendo dados sensíveis dos pacientes e garantindo conformidade com regulamentações de segurança.

3. **Usabilidade**: A interface do sistema deve ser intuitiva e amigável, facilitando o aprendizado e uso por parte dos funcionários da clínica.

4. **Compatibilidade**: O sistema deve funcionar adequadamente em diferentes dispositivos (desktops e tablets) e navegadores.

5. **Confiabilidade**: O sistema deve ser estável, com tempo de inatividade mínimo e mecanismos para recuperação de dados em caso de falhas.

6. **Escalabilidade**: O sistema deve suportar o crescimento do número de dentistas, pacientes e consultas sem degradação de desempenho.

7. **Manutenibilidade**: O código deve ser organizado e documentado para facilitar futuras atualizações e expansões do sistema.

8. **Portabilidade**: O sistema deve ser desenvolvido como uma aplicação web responsiva, permitindo acesso de diferentes dispositivos e plataformas.

## Restrições

1. O sistema atenderá apenas uma única unidade da clínica (não multi-clínica).
2. O sistema apenas registra informações financeiras; não realiza cobranças ou integrações bancárias.
3. Anexos no prontuário devem respeitar limites de tamanho e tipos de arquivo compatíveis (ex: PDF, JPG, PNG).
