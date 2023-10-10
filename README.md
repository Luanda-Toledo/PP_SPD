# Contador de 7 Segmentos con Botones

Este proyecto Arduino implementa un contador de 7 segmentos que muestra un número y permite incrementarlo o decrementarlo utilizando botones. El contador puede mostrar números del 0 al 99 en dos displays de 7 segmentos. El código utiliza una técnica de multiplexación para controlar los displays y gestionar los botones.

![image](https://github.com/Luanda-Toledo/PP_SPD/assets/58377353/1dbeda31-8623-469e-95d6-d87a722e7016)

## Requisitos de Hardware

- Placa Arduino (se ha probado en Arduino Uno)
- Dos displays de 7 segmentos comunes anodo
- Tres botones (para suma, resta y reset)
- Resistencias pull-up (10kΩ) para los botones
- Cables y protoboard para la conexión

## Conexiones

- Conecta los displays de 7 segmentos a los pines A4 (UNIDAD) y A5 (DECENA) de la placa Arduino.
- Conecta los segmentos de los displays a los pines 7 (C), 8 (D), 9 (E), 10 (G), 11 (F), 12 (A), y 13 (B) de la placa Arduino.
- Conecta un botón a los pines 3 (ENTRADA_RESTA), 4 (ENTRADA_SUMA) y 5 (ENTRADA_RESET) de la placa Arduino. Utiliza resistencias pull-up (10kΩ) para los pines de entrada de los botones.

## Uso

1. Cargue el código en su Arduino utilizando el IDE de Arduino.
2. Conecte los componentes siguiendo las conexiones descritas anteriormente.
3. Presione el botón de suma (+) para incrementar el contador.
4. Presione el botón de resta (-) para decrementar el contador.
5. Presione el botón de reset para volver a cero.

## Notas Adicionales

- El código utiliza una técnica de multiplexación para alternar entre los displays de decenas y unidades.
- El contador se reinicia automáticamente a 0 cuando alcanza 99 o se decrementa por debajo de 0.
- Se utiliza una resistencia pull-up interna para los pines de entrada de los botones.

## Integrantes
- Yanina Bonelli
- Matias Caballero

## Link al proyecto
https://www.tinkercad.com/things/04xtZsmu38V



