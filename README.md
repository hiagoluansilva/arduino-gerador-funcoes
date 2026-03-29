# arduino-gerador-funcoes

Gerador de funções com 4 formas de onda no ESP32 usando DAC e interrupção de timer.

## Descrição

Gerador de formas de onda que utiliza o DAC interno do ESP32 para produzir sinais analógicos a partir de tabelas de lookup com 112 amostras. A saída é atualizada por uma ISR de timer de hardware para frequência precisa e estável.

## Hardware

- Placa: ESP32
- Saída DAC: GPIO 25 (seno), GPIO 26 (triangular)

## Formas de onda disponíveis

| Índice | Forma |
|--------|-------|
| 0 | Senoidal |
| 1 | Triangular |
| 2 | Dente de Serra |
| 3 | Quadrada |

## Parâmetros

- **Amostras:** 112 pontos por ciclo
- **Resolução DAC:** 8 bits (0–255)
- **Prescaler timer:** 255 → ~312 kHz → ~2,8 kHz por forma de onda

## Como usar

1. Abra `gerador_de_func.ino` no Arduino IDE
2. Selecione **ESP32 Dev Module**
3. Altere `wave_type` (0–3) para escolher a forma de onda
4. Compile e grave

## Escola

Centro Tecnológico Liberato — Novo Hamburgo/RS
