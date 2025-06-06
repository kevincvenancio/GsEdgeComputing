# 🌊 LNK Tech - Sistema de Alerta de Enchentes

## 📍 Descrição do Problema

As enchentes urbanas representam uma ameaça recorrente em diversas regiões do Brasil, ocasionando alagamentos de ruas, destruição de patrimônio, perdas econômicas e riscos à vida. Fatores como chuvas intensas, falhas no sistema de drenagem e a ausência de monitoramento em tempo real dificultam ações preventivas eficazes.

Existe, portanto, uma demanda urgente por sistemas de alerta **acessíveis, confiáveis e de fácil implementação**, especialmente voltados para comunidades carentes, que são as mais afetadas por esses desastres naturais.

## 💡 Visão Geral da Solução

A **LNK Tech** propõe um **sistema físico inteligente de monitoramento ambiental**, voltado à **prevenção de enchentes em áreas de risco**. O projeto utiliza sensores para detectar, em tempo real, variáveis críticas como:

- Intensidade da chuva
- Umidade relativa do ar
- Nível da água
- Fluxo de líquidos

Com base nas leituras dos sensores, o sistema **aciona alertas visuais (LEDs)** e **sonoros (buzzer)**, além de simular o funcionamento de uma bomba d'água, ajudando a alertar a população e autoridades de maneira simples e eficaz.

### 🧩 Componentes Utilizados

- **Sensor DHT22** – mede temperatura e umidade do ar  
- **Sensor ultrassônico** – detecta o nível da água  
- **Potenciômetro** – simula a intensidade da chuva  
- **Sensor de fluxo** – simulado via entrada analógica (A1)  
- **LEDs (verde, amarelo, vermelho)** – indicam o nível de risco  
- **Buzzer** – emite alertas sonoros em situações críticas  
- **Display LCD I2C 16x2** – exibe informações e mensagens de status  
- **LED RGB** – simula o acionamento de uma bomba d’água

### ⚙️ Funcionamento

O sistema opera com base em quatro níveis de alerta, definidos pela leitura combinada dos sensores:

- **🌤️ Sem chuva**: sistema em modo de repouso; LED verde ligado.  
- **🌦️ Chuva fraca ou moderada**: LED amarelo aceso; sem alarme sonoro.  
- **🌧️ Risco de enchente**: LED vermelho aceso; buzzer intermitente; alerta no LCD.  
- **🌊 Nível de água crítico**: LED vermelho piscando; buzzer contínuo; LED RGB ligado simulando bomba de escoamento.

### 🖼️ Ilustração

A seguir, uma representação esquemática do circuito desenvolvido:

![Diagrama do sistema](img/diagrama.png)

```
[ DHT22 ]      [ ULTRASSÔNICO ]
    |                 |
    |                 |
[ LCD ] -- [ ARDUINO UNO ] -- [ LEDs / Buzzer / Sensores ]
```

## 🧪 Como Simular o Projeto

A simulação pode ser feita gratuitamente na plataforma online **Wokwi**, especializada em prototipagem de sistemas Arduino.

### Passo a passo:

1. Acesse o projeto: [Simulação no Wokwi](https://wokwi.com/projects/432149335150942209)
2. Clique em **"Start Simulation"**.
3. Observe os dados exibidos no **LCD** e no **console serial**.
4. Ajuste o **potenciômetro** para simular diferentes intensidades de chuva.
5. Mova o objeto diante do **sensor ultrassônico** para simular variações no nível da água.

### 🔗 Link Direto para a Simulação

(https://wokwi.com/projects/432149335150942209)

### 🎥 Vídeo Demonstrativo

*Link será adicionado em breve.*

## 👨‍💻 Integrantes do Grupo

- **Kevin Carvalho Venancio** – RM: 561459  
- **Nicolas Barnabe da Cruz** – RM: 561997  
- **Luiz Antônio Morais** – RM: 562142
