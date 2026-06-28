## 📄 README PRINCIPAL

```markdown
# 🔬 ESP32 Sensor Lab

![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)
![Platform](https://img.shields.io/badge/platform-ESP32-blue)
![Language](https://img.shields.io/badge/language-C++-orange)

> **"Aprender na prática, um sensor de cada vez"**

## 🎯 Objetivo

Este repositório é meu laboratório pessoal para testar e entender o funcionamento de sensores, atuadores e módulos com ESP32. Cada teste é documentado com:

- 📋 Esquema de ligação (pinagem)
- 💻 Código-fonte comentado
- 📊 Exemplos de saída/serial
- 🧪 Observações e aprendizados
- 💡 Ideias de aplicação prática

## 📦 Sensores/Atuadores Testados

### ✅ Concluídos

| Sensor/Atuador | Descrição | Data | Link |
|----------------|-----------|------|------|
| PN5180 - NFC | Leitor de tags NFC via protocolo SPI | 28/06/2026 | [📁](./sensors/01-pn5180-nfc/) |
| *Adicione mais* | *conforme testar* | *...* | *...* |

### ⏳ Em andamento

- [ ] Sensor ultrassônico HC-SR04
- [ ] ex. Display OLED SSD1306
- [ ] ex. Sensor de temperatura DS18B20
- [ ] ex. Módulo relê
- [ ] ex. Câmera ESP32-CAM
- [ ] *Adicione os seus*

### 📋 Planejados

- [ ] Módulo Bluetooth HC-05
- [ ] Sensor de gás MQ-2
- [ ] Servo motor
- [ ] Sensor de cor TCS3200
- [ ] Módulo RFID RC522
- [ ] Sensor de luminosidade LDR
- [ ] Sensor de efeito Hall
- [ ] Módulo GPS NEO-6M
- [ ] Acelerômetro MPU6050

## 🗂️ Estrutura do Repositório

```plaintext
esp32-sensor-lab/
├── sensors/
│   ├── 01-pn5180-nfc/
│   │   ├── README.md          # Documentação completa do teste
│   │   └── pn5180-test.ino    # Código-fonte Arduino
│   ├── 02-proximo-sensor/
│   │   ├── README.md
│   │   └── codigo.ino
│   └── ... (mais sensores)
├── libraries/                 # Libs customizadas (se houver)
├── utils/                     # Funções auxiliares
├── docs/                      # Documentação geral
│   ├── pinout-esp32.md       # Mapeamento de pinos
│   └── wiring-guide.md       # Guia de ligações
├── .gitignore
├── LICENSE
└── README.md
```

## 🔧 Pré-requisitos

### Hardware
- ESP32 (qualquer modelo: DevKit, NodeMCU, ESP32-WROOM, etc.)
- Cabo USB (micro-USB ou USB-C)
- Protoboard e jumpers
- Componentes conforme cada teste

### Software
- Arduino IDE (versão 1.8.19 ou superior) ou PlatformIO
- Biblioteca ESP32 instalada (via Gerenciador de Placas)
- Drivers USB para o ESP32
- Bibliotecas específicas conforme cada teste

### Instalação do ESP32 na Arduino IDE

1. Abra a Arduino IDE
2. Vá em **Arquivo > Preferências**
3. Em "URLs Adicionais para Gerenciadores de Placas", adicione:
   ```
   https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json
   ```
4. Vá em **Ferramentas > Placa > Gerenciador de Placas**
5. Procure por "ESP32" e instale

## 🚀 Como Usar

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/esp32-sensor-lab.git
```

2. Navegue até a pasta do sensor desejado:
```bash
cd esp32-sensor-lab/sensors/01-pn5180-nfc
```

3. Abra o arquivo `.ino` na Arduino IDE

4. Conecte o ESP32 e selecione a placa correta:
   - **Ferramentas > Placa > ESP32 Dev Module**
   - **Ferramentas > Porta** (selecione a porta correta)

5. Faça o upload do código

6. Abra o Monitor Serial (115200 baud)

## 📝 Padrão de Documentação

Cada teste segue o formato:

```markdown
# [Nome do Sensor]

## 📋 Informações
- **Modelo:** [ex: PN5180]
- **Tensão:** [ex: 3.3V/5V]
- **Protocolo:** [ex: SPI/I2C/OneWire]

## 🔌 Esquema de Ligação
| Pino Sensor | Pino ESP32 |
|-------------|------------|
| VCC         | 3.3V/5V   |
| GND         | GND        |
| SCLK        | GPIO 18    |
| MOSI        | GPIO 23    |

## 💻 Código
[Código-fonte com explicações]

## 📊 Exemplo de Saída
```
[Saída do Monitor Serial]
```

## 💡 Aplicações Práticas
- [Ideia 1]
- [Ideia 2]

## ⚠️ Observações
- [Dificuldades encontradas]
- [Dicas importantes]
```

## 🎓 Aprendizados ao Longo da Jornada

*Esta seção será atualizada conforme os testes avançam*

### Lições Aprendidas

- **Conexões:** Sempre verificar a tensão correta (3.3V vs 5V) antes de conectar
- **Protocolos:** SPI precisa de pinos específicos, I2C precisa de pull-ups
- **Documentação:** Salvar sempre os esquemas de ligação para referência futura

## 🤝 Contribuição

Este é um repositório pessoal de aprendizado, mas sugestões são bem-vindas!

1. Faça um fork do projeto
2. Crie sua branch (`git checkout -b feature/novo-sensor`)
3. Commit suas mudanças (`git commit -m 'feat: adiciona novo sensor'`)
4. Push para a branch (`git push origin feature/novo-sensor`)
5. Abra um Pull Request

## 📚 Referências Gerais

- [ESP32 Datasheet](https://www.espressif.com/sites/default/files/documentation/esp32_datasheet_en.pdf)
- [Arduino ESP32 Core - Documentação](https://docs.espressif.com/projects/arduino-esp32/en/latest/)
- [Random Nerd Tutorials](https://randomnerdtutorials.com/)
- [ESP32 Pinout Reference](https://lastminuteengineers.com/esp32-pinout-reference/)

## 📄 Licença

Este projeto está sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.

---

⭐ **Progresso:** 1/XX sensores testados

*Última atualização: 28/06/2026*
```

---
