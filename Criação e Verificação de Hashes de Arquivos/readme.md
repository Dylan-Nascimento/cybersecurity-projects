# Criação e Verificação de Hashes de Arquivos

## Descrição

Neste laboratório, você criará e avaliará os valores de hash de dois arquivos. Utilizando comandos do Linux, será possível calcular os hashes e compará-los para determinar se os arquivos são iguais ou diferentes — uma técnica fundamental em verificação de integridade e segurança da informação.

## Tecnologias Utilizadas

- **Plataforma**: Google Cloud Skillboost
- **Sistema Operacional**: Linux
- **Ferramentas/Comandos**: `sha256sum`, `cmp`, `cat`, `ls`

## Passos do Laboratório

1. **Introdução**: Acessar o ambiente provisionado pela plataforma Cloud Skillboost com os arquivos prontos para análise.

2. **Configuração do ambiente**:

   - O diretório de trabalho atual é `/home/analyst`.
   - Dois arquivos de texto estão disponíveis: `file1.txt` e `file2.txt`.
   - Acesso ao terminal Linux via navegador.

3. **Execução**:

   ### Tarefa 1. Gerar hashes para arquivos

   1. Use o comando `ls` para listar o conteúdo do diretório:
      ```bash
      ls
      ```
      - Saída esperada: `file1.txt  file2.txt`

   2. Use o comando `cat` para exibir o conteúdo do arquivo `file1.txt`:
      ```bash
      cat file1.txt
      ```

   3. Use o comando `cat` para exibir o conteúdo do arquivo `file2.txt`:
      ```bash
      cat file2.txt
      ```

   4. Analise a saída do conteúdo dos dois arquivos.

   5. Use o comando `sha256sum` para gerar o hash do arquivo `file1.txt`:
      ```bash
      sha256sum file1.txt
      ```

   6. Use o comando `sha256sum` para gerar o hash do arquivo `file2.txt`:
      ```bash
      sha256sum file2.txt
      ```

   7. Revise os hashes gerados do conteúdo dos dois arquivos.

   ### Tarefa 2. Comparar hashes

   1. Use o comando `sha256sum` para gerar o hash do arquivo `file1.txt` e enviar a saída para um novo arquivo chamado `file1hash`:
      ```bash
      sha256sum file1.txt > file1hash
      ```

   2. Use o comando `sha256sum` para gerar o hash do arquivo `file2.txt` e enviar a saída para um novo arquivo chamado `file2hash`:
      ```bash
      sha256sum file2.txt > file2hash
      ```

   3. Use o comando `cat` para exibir os valores de hash nos arquivos `file1hash` e `file2hash`:
      ```bash
      cat file1hash
      cat file2hash
      ```

   4. Inspecione a saída e observe a diferença nos valores de hash.

   5. Use o comando `cmp` para destacar as diferenças nos arquivos `file1hash` e `file2hash`:
      ```bash
      cmp file1hash file2hash
      ```

   6. Examine a saída, que informa a primeira diferença entre os dois arquivos.

4. **Conclusão**:

   Este laboratório reforça o entendimento sobre o uso de funções hash para verificar a integridade de arquivos, destacando a importância dessas ferramentas na cibersegurança.

## Prints de Tela

### Execução dos comandos `sha256sum` e visualização de conteúdo

### Redirecionamento de hash para arquivos e comparação com `cmp`

**Nota**: Este laboratório faz parte do curso de certificação em cibersegurança do Google, utilizando a plataforma Cloud Skillboost.

