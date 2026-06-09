# ForestEye

Sistema de monitoramento de risco de queimadas desenvolvido com Arduino.

## Componentes

- Arduino Uno
- DHT22
- LDR
- LCD 16x2
- LEDs (verde, amarelo e vermelho)
- Buzzer

## Funcionamento

### Risco Baixo
- Temperatura < 28°C
- Umidade >= 30%
- Luminosidade < 60%

### Risco Médio
- Temperatura >= 28°C
ou
- Luminosidade >= 60%
ou
- Umidade < 30%

### Risco Alto
- Temperatura >= 38°C
- Luminosidade >= 60%
- Umidade < 30%

## Simulação
Projeto desenvolvido para execução no Wokwi.
