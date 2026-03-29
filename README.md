# Arduino Gerador de Funções — 4 Formas de Onda (ESP32)

🇧🇷 **Português** | 🇺🇸 [English](#english)

---

## Português

Gerador de funções no ESP32 com 4 formas de onda (senoidal, quadrada, triangular, dente-de-serra), 112 amostras por ciclo, saída via DAC nos GPIO25/GPIO26 e ISR de timer.

### O que faz
- Gera 4 formas de onda: **senoidal, quadrada, triangular, dente-de-serra**
- **112 amostras** por ciclo para boa resolução de forma
- Saída via **DAC** nos pinos **GPIO25** e **GPIO26**
- Timer ISR com **PSC = 255** controla a taxa de atualização das amostras
- Forma de onda selecionável por botão ou variável

### Parâmetros
| Parâmetro | Valor |
|---|---|
| Amostras por ciclo | 112 |
| Formas de onda | 4 (sin, sqr, tri, saw) |
| Saída DAC 1 | GPIO25 |
| Saída DAC 2 | GPIO26 |
| Timer PSC | 255 |

### Plataforma
ESP32 — Arduino Framework (DAC interno de 8 bits)

---

## English

Function generator on ESP32 with 4 waveforms (sine, square, triangle, sawtooth), 112 samples per cycle, DAC output on GPIO25/GPIO26, and timer ISR.

### What it does
- Generates 4 waveforms: **sine, square, triangle, sawtooth**
- **112 samples** per cycle for good waveform resolution
- Output via **DAC** on pins **GPIO25** and **GPIO26**
- Timer ISR with **PSC = 255** controls sample update rate
- Waveform selectable by button or variable

### Parameters
| Parameter | Value |
|---|---|
| Samples per cycle | 112 |
| Waveforms | 4 (sin, sqr, tri, saw) |
| DAC output 1 | GPIO25 |
| DAC output 2 | GPIO26 |
| Timer PSC | 255 |

### Platform
ESP32 — Arduino Framework (8-bit internal DAC)
