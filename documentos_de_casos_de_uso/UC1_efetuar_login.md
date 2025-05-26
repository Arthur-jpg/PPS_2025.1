# Caso de Uso: Efetuar Login

**Atores:** Secretaria, Dentista

**Descrição:**
Permite que usuários autorizados (secretária e dentistas) acessem o sistema da clínica odontológica por meio de autenticação, garantindo o controle de acesso conforme o perfil do usuário.

**Fluxo Principal:**
1. O usuário acessa a tela de login do sistema.
2. Informa suas credenciais (usuário e senha).
3. O sistema valida as credenciais.
4. O sistema libera o acesso conforme o perfil (secretária ou dentista).

**Fluxos Alternativos:**
- Se as credenciais estiverem incorretas, o sistema exibe mensagem de erro e solicita nova tentativa.

**Pré-condições:**
- O usuário deve estar cadastrado no sistema.

**Pós-condições:**
- O usuário tem acesso às funcionalidades permitidas pelo seu perfil.
