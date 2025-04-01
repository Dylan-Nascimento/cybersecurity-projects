
# Monitoramento e Análise de Logs com Splunk Cloud

## Descrição

O objetivo deste laboratório é explorar as funções do Splunk Cloud, utilizando indexação, consulta e monitoramento de logs.

## Tecnologias Utilizadas

- **Plataforma**: Splunk Cloud
- **Sistema Operacional**: Baseado em nuvem
- **Ferramentas**: Splunk Search Processing Language (SPL)
- **Linguagens**: SPL, Bash (quando necessário)

## Passos do Laboratório

1. **Introdução**: Configurar uma conta no Splunk Cloud e utilizar a interface para consultas.

2. **Configuração do ambiente**:

   - O ambiente será configurado acessando o Splunk Cloud.
   - Criar uma conta de avaliação gratuita.
   - Explorar os logs disponíveis no ambiente de laboratório e entender como eles são indexados para análise.

3. **Execução**: 

   - **Tarefa 1:** Pesquisar dados indexados no Splunk Cloud.

   - **Tarefa 2:** Avaliar resultados da pesquisa (eventos e possíveis incidentes).

   - **Tarefa 3:** Explorar as diferentes fontes de logs já disponíveis no ambiente.

   - **Tarefa 4:** Localizar login(s) SSH com falha para a conta root.

4. **Conclusão**: Após este laboratório, o usuário terá desenvolvido experiência prática no uso do Splunk Cloud para indexação, consulta e monitoramento de logs.

### **Comandos Utilizados**

```spl
# Pesquisar todos os logs indexados no índice principal
index="main"

# Filtrar os resultados para eventos do servidor de e-mail
index=main host=mailsv 

# Filtrar logins SSH com falha para a conta root
index=main host=mailsv fail* root
```

## Prints de Tela

### Pesquisar por dados indexados

### Avaliar resultados de pesquisa

### Explorar diferentes fontes de logs disponíveis

### Localizar login(s) SSH com falha para a conta root

**Nota**: Este é um laboratório realizado como parte do curso de certificação em cibersegurança do Google.

