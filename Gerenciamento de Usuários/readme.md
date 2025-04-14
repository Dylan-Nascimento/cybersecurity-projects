# Gerenciamento de Usuários no Sistema com Cloud Skillboost

## Descrição

O objetivo deste laboratório é aprender a adicionar um usuário, adicioná-lo a um grupo, alterar permissões em arquivos e remover o usuário em um sistema Linux utilizando a interface de terminal provida pela plataforma Cloud Skillboost.

## Tecnologias Utilizadas

- **Plataforma**: Google Cloud Skillboost
- **Sistema Operacional**: Linux (Debian/Ubuntu)
- **Ferramentas**: Terminal Bash
- **Linguagens**: Shell Script / Bash

## Passos do Laboratório

1. **Introdução**: Acessar o ambiente provisionado pela plataforma Cloud Skillboost e abrir o terminal.

2. **Configuração do ambiente**:

   - O ambiente é provisionado automaticamente pela plataforma Cloud Skillboost.
   - Acesso ao terminal com permissões de superusuário (root ou sudo).
   - Todos os pacotes necessários já estão instalados.

3. **Execução**:

   - **Tarefa 1:** Adicionar um novo usuário ao sistema.

     - **Código Utilizado:**
       ```bash
       sudo useradd researcher9
       ```
     - **Resultado:** Usuário researcher9 adicionado com sucesso.

   - **Tarefa 2:** Adicionar o usuário a um grupo.

     - **Código Utilizado:**
       ```bash
       sudo usermod -g research_team researcher9
       ```
     - **Resultado:** Usuário researcher9 adicionado ao grupo research\_team com sucesso.

   - **Tarefa 3:** Alterar permissões de usuário em arquivos.

     - **Código Utilizado:**
       ```bash
       sudo chown researcher9 /home/researcher2/projects/project_r.txt
       ```
     - **Resultado:** Permissões de acesso ao project\_r.txt atualizadas para o usuário researcher9.

   - **Tarefa 4:** Remover um usuário do sistema.

     - **Código Utilizado:**
       ```bash
        sudo userdel researcher9
       userdel: group researcher9 not removed because it is not the primary group of user researcher9.
       sudo groupdel researcher9
       ```
     - **Resultado:** Usuário researcher9 removido com sucesso.

4. **Conclusão**: Após este laboratório, o usuário terá aprendido os comandos básicos para gerenciar contas de usuários em um sistema Linux, incluindo adição, associação a grupos, modificação de permissões e remoção.

## Prints de Tela

### Adicionar um novo usuário

### Adicionar o usuário a um grupo

### Alterar permissões de usuário em arquivos

### Remover um usuário

**Nota**: Este é um laboratório realizado como parte do curso de certificação em cibersegurança do Google, utilizando a plataforma Cloud Skillboost.





