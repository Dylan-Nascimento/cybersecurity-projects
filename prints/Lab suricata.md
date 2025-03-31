# Alertas, logs e regras com Suricata

## Descrição

O objetivo deste laboratório é explorar as funções do Suricata e aprender a configurar e disparar alertas.

## Tecnologias Utilizadas

- **Plataforma**: Cloud Skill Boost (Google Cloud)
- **Sistema Operacional**: Linux/Ubuntu
- **Ferramentas**: Suricata
- **Linguagens**: Bash

## Passos do Laboratório

1. **Introdução**: Examinar uma regra, praticar o uso do Suricata para disparar alertas no tráfego de rede e analisar saídas de log.

2. **Configuração do ambiente**:

   - O ambiente é configurado automaticamente pelo Cloud Skill Boost.
   - Todas as ferramentas necessárias já estão instaladas e prontas para uso.
   - Basta acessar o Google Cloud Shell e executar os comandos conforme instruído no laboratório.

3. **Execução**: 

   - **Tarefa 1:** Exibir a regra no arquivo **custom.rules**

   - **Tarefa 2:** Acionar essa regra e examinar os logs de alerta que o Suricata gera.

   - **Tarefa 3:** Examinar a saída adicional que o Suricata gera em um arquivo **JSON**.

4. **Conclusão**: Experiência prática na execução do Suricata para

   criar regras personalizadas e executá-las e monitorar o tráfego capturado em um arquivo de captura de pacote e

   examinar a saída do arquivo JSON.

### **Comandos Utilizados**

```sh
# Exibir a regra no arquivo custom.rules
cat custom.rules

# Acionar a regra e examinar os logs de alerta

ls -l /var/log/suricata

sudo suricata -r sample.pcap -S custom.rules -k none

ls -l /var/log/suricata

cat /var/log/suricata/fast.log

# Examinar a saída do Suricata em JSON

cat /var/log/suricata/eve.json

jq . /var/log/suricata/eve.json | less

jq -c "[.timestamp,.flow_id,.alert.signature,.proto,.dest_ip]" /var/log/suricata/eve.json

jq "select(.flow_id==X)" /var/log/suricata/eve.json
```

## Prints de Tela

### Exibindo a regra no arquivo `custom.rules`



### Logs de alerta gerados pelo Suricata



### Saída do arquivo JSON



> **Nota**: Este é um laboratório realizado como parte do curso de certificação em cibersegurança do Google.

