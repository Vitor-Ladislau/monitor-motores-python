# monitor-motores-python
Trabalho prático avaliativo sobre versionamento GitHUB e VScode

# Relatório em MarkDown sobre o funcionamento do código 📋
## Código de Monitor Industrial:

Esse código foi desenvolvido com o intuito de monitorar os motores industriais por meio de: **Painel de Telemetria e Análise de Criticidade**. 🧑🏾‍🏭

## Esse sistema primeiramente vai te dizer quais são os motores industriais listados nele e seus respectivos setores: 

- MTR-01
Estamparia

- MTR-02
Usinagem

- MTR-03
Bobinagem

- MTR-04
Pintura

### O código demonstra nas estatísticas Operacionais da Planta: _O Total de Motores, A Temperatura Média, A Corrente Média, A Potência Total e o Motor mais quente._ 
---
## Ele também lista um plano de manutenção preventiva demonstrando se algum motor precisa ser interrompido, atenção ou se pode continuar operando normalmente:

Plano de Manutenção Preventiva (Closes #1)
🛑 Parada Imediata (CRÍTICO)
Motores com 2 ou mais parâmetros fora do limite operacional:

['MTR-02'] — Usinagem (3 ocorrências)
⚠️ Inspeção Programada (ATENÇÃO)
Motores com 1 parâmetro fora do limite operacional:

['MTR-03'] — Bobinagem (1 ocorrência)
✅ Operação Estável (NORMAL)
Motores operando dentro de todos os limites:

['MTR-01', 'MTR-04']

---

### Na parte de Leituras dos Sensores e Diagnóstico o código nos mostra uma tabela como demonstrado abaixo:


Status | ID / Setor | Temperatura | Corrente | Vibração | Rotação | Potência | Alertas Detectados
-- | -- | -- | -- | -- | -- | -- | --
NORMAL | MTR-01Estamparia | 68.4 °C | 14.2 A | 2.1 mm/s | 1750 RPM | 7.5 kW | Nenhuma ocorrência
CRÍTICO | MTR-02Usinagem | 84.7 °C | 19.3 A | 5.2 mm/s | 1690 RPM | 11.0 kW | • Superaquecimento (84.7 °C)• Sobrecorrente (19.3 A)• Vibração elevada (5.2 mm/s)
ATENÇÃO | MTR-03Bobinagem | 76.2 °C | 17.8 A | 4.7 mm/s | 1520 RPM | 5.5 kW | • Vibração elevada (4.7 mm/s)
NORMAL | MTR-04Pintura | 61.0 °C | 11.5 A | 1.8 mm/s | 1780 RPM | 7.5 kW | Nenhuma ocorrência

## Então com este programa você pode definir os motores que estão apresentando uma temperatura ideal conforme o limite proposto:
### **Limites: Temp ≤ 80°C** ♨️

- [x]  MTR-01
- [ ]  MTR-02
- [x] MTR-03
- [x] MTR-04

## Pode também ranquea-los conforme sua potência⚡

1. MTR-02
2. MTR-01
3. MTR-04
4. MTR-03
