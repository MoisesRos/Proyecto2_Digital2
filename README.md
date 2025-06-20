# Proyecto 2 - Fly Bros: Videojuego con Controles Inalámbricos

![Plataforma](https://img.shields.io/badge/Plataforma-STM32F446RE/Nucleo-blue) 
![Controles](https://img.shields.io/badge/Controles-PS4/ESP32-green) 
![Pantalla](https://img.shields.io/badge/Display-ILI9341_SPI-orange) 
![UVG](https://img.shields.io/badge/Universidad-UVG-red)

## Resumen General
Implementación de un videojuego arcade estilo "Fly Bros" con:
- **Controles inalámbricos PS4** mediante ESP32
- **Renderizado gráfico** en pantalla TFT ILI9341
- **Sistema de sonido** 8-bit con DAC y buzzer
- **Persistencia de datos** en tarjeta SD
- **Arquitectura cliente-servidor** entre dispositivos

 ## Características Principales

### 1. Arquitectura del Sistema
PS4-->|Bluetooth| ESP32
    ESP32-->|UART| NUCLEO[NUCLEO-F446RE]
    NUCLEO-->|SPI| TFT[Pantalla ILI9341]
    NUCLEO-->|SPI| SD[Memoria SD]
    NUCLEO-->|DAC| BUZZER[Buzzer Pasivo]
