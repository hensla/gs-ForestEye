📖 Descrição do Projeto

O ForestEye é um sistema embarcado desenvolvido com Arduino para monitorar condições ambientais relacionadas ao risco de queimadas e incêndios florestais.

A solução utiliza sensores de temperatura, umidade do ar e luminosidade para calcular um índice de risco em tempo real. Com base nos dados coletados, o sistema alerta o usuário por meio de LEDs, buzzer e mensagens exibidas em um display LCD.

O projeto busca demonstrar como tecnologias de baixo custo podem ser utilizadas para auxiliar na prevenção e monitoramento de eventos ambientais que causam impactos significativos ao meio ambiente.

🎯 Objetivo da Solução

O principal objetivo do projeto é identificar condições que favorecem o surgimento de queimadas, fornecendo alertas visuais e sonoros para facilitar a tomada de decisões preventivas.

A solução foi desenvolvida para:

Monitorar temperatura ambiente.
Monitorar umidade relativa do ar.
Monitorar níveis de luminosidade.
Classificar o risco de queimadas em três níveis.
Emitir alertas automáticos ao detectar situações críticas.
Demonstrar a aplicação prática de sensores e sistemas embarcados na área ambiental.
🔧 Componentes Utilizados
Componente	Quantidade
Arduino Uno	1
Sensor DHT22	1
Sensor LDR (Fotoresistor)	1
Display LCD 16x2	1
Potenciômetro 10kΩ	1
LED Verde	1
LED Amarelo	1
LED Vermelho	1
Buzzer	1
Resistores 220Ω	3
Resistores 10kΩ	2
Protoboard	1
Jumpers	Diversos
⚙️ Explicação do Funcionamento

O sistema realiza a leitura contínua dos sensores conectados ao Arduino:

🌡 Temperatura e Umidade

O sensor DHT22 é responsável por medir:

Temperatura ambiente (°C)
Umidade relativa do ar (%)
☀️ Luminosidade

O sensor LDR mede a intensidade luminosa do ambiente.

Os valores lidos são convertidos para uma escala percentual de 0% a 100%.

🚦 Classificação do Risco

O sistema classifica o ambiente em três níveis de risco:

🟢 Risco Baixo

Condições:

Temperatura abaixo de 28°C
Luminosidade abaixo de 60%
Umidade acima de 30%

Resposta:

LED verde aceso
LCD exibe "RISCO BAIXO"
Buzzer desligado
🟡 Risco Médio

Condições:

Temperatura maior ou igual a 28°C

OU

Luminosidade maior ou igual a 60%

OU

Umidade inferior a 30%

Resposta:

LED amarelo aceso
LCD exibe "RISCO MEDIO"
Buzzer desligado
🔴 Risco Alto

Condições:

Temperatura maior ou igual a 38°C
Luminosidade maior ou igual a 60%
Umidade inferior a 30%

Resposta:

LED vermelho aceso
Buzzer ativado
LCD exibe "RISCO ALTO"
🔌 Estrutura do Circuito
Sensor DHT22
Pino DHT22	Arduino
VCC	5V
DATA	D2
GND	GND
Sensor LDR
Pino	Arduino
AO	A0
VCC	5V
GND	GND
LEDs
LED	Pino
Verde	D8
Amarelo	D9
Vermelho	D10
Buzzer
Componente	Pino
Buzzer	D11
LCD 16x2
LCD	Arduino
RS	D7
E	D6
D4	D5
D5	D4
D6	D3
D7	D12

▶️ Instruções de Execução
Executando no Wokwi
Acesse o site do Wokwi.
Crie um novo projeto Arduino Uno.
Adicione os componentes:
DHT22
LDR
LCD 16x2
Potenciômetro
LEDs
Buzzer

Configure as conexões conforme a tabela apresentada.
Copie o código-fonte para o arquivo sketch.ino.
Inicie a simulação clicando em Start Simulation.
Altere os valores dos sensores para testar os diferentes níveis de risco.

🌱 Impacto Ambiental

O projeto contribui para a conscientização sobre monitoramento ambiental e prevenção de queimadas, demonstrando como sensores e sistemas embarcados podem auxiliar na identificação precoce de situações de risco.

Henry Ferreira 
Renan Lopes
Lucas Mazzeo
Eduardo Arruda 
Henrique Massoco
