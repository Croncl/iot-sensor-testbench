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
| :--- | :--- | :--- | :--- |
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
│   ├── pinout-esp32.md        # Mapeamento de pinos
│   └── wiring-guide.md        # Guia de ligações
├── .gitignore
├── LICENSE
└── README.md
