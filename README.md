# Projeto de Performance - JSONPlaceholder API

Projeto de testes de performance desenvolvido com Apache JMeter, simulando cenários reais de carga contra a API pública JSONPlaceholder.

## Tecnologias utilizadas
- Apache JMeter 5.6.3
- Java JDK 25
- JSONPlaceholder API (https://jsonplaceholder.typicode.com)

## Cenários de teste
- **Teste de carga:** 10 usuários simultâneos, ramp-up de 5 segundos, 3 iterações (30 requisições no total)
- **Endpoint testado:** GET /posts

## Resultados obtidos
| Métrica | Valor |
|---|---|
| Total de requisições | 30 |
| Taxa de erro | 0.00% |
| Tempo médio de resposta | 152ms |
| Tempo mínimo | 86ms |
| Tempo máximo | 571ms |
| Percentil 90 (P90) | 246ms |
| Percentil 95 (P95) | 396ms |
| Throughput | 6.19 req/s |
| APDEX | 0.983 |

## Como executar
1. Instale o Java JDK 11+
2. Baixe o Apache JMeter em https://jmeter.apache.org
3. Clone este repositório
4. Execute via terminal:

    jmeter -n -t "Projeto Portfolio - JSONPlaceholder API.jmx" -l resultados.jtl -e -o relatorio

5. Abra a pasta relatorio/index.html no navegador

## Relatório
O relatório HTML completo está disponível na pasta /relatorio