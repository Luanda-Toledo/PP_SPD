# Control de Velocidad de Ventilador con Sensor de Temperatura

Este proyecto de Arduino Uno en Tinkercad te permite controlar la velocidad de un ventilador de acuerdo con la temperatura ambiente. Cuando la temperatura aumenta, el ventilador gira más rápido para enfriar el entorno. Además, muestra la temperatura en un display de 7 segmentos.

![image](https://github.com/Luanda-Toledo/PP_SPD/assets/58377353/a094c25c-922f-48fc-9db3-8f0028f88ba1)

## Requisitos de Hardware

- Placa Arduino (se ha probado en Arduino Uno)
- Dos displays de 7 segmentos comunes anodo (para mostrar la temperatura)
- Resistencias pull-up (10kΩ) para los botones
- Cables y protoboard para la conexión
- Un interruptor
- Sensor de temperatura (analogico)
- Motor CC
  
## Conexiones

- Conecta los displays de 7 segmentos a los pines A4 (UNIDAD) y A5 (DECENA) de la placa Arduino.
- Conecta los segmentos de los displays a los pines 7 (C), 8 (D), 9 (E), 10 (G), 11 (F), 12 (A), y 13 (B) de la placa Arduino.
- Conecta un botón a los pines 3 (ENTRADA_RESTA), 4 (ENTRADA_SUMA) y 5 (ENTRADA_RESET) de la placa Arduino. Utiliza resistencias pull-up (10kΩ) para los pines de entrada de los botones.
- Conecta el interruptor o pulsador al pin ENTRADA_INTERRUPTOR. Utiliza resistencias pull-up (10kΩ).

## Uso

1. Cargue el código en su Arduino utilizando el IDE de Arduino.
2. Conecte los componentes siguiendo las conexiones descritas anteriormente.
3. Enciende el interruptor para activar el sistema. El ventilador comenzará a funcionar y la temperatura se mostrará en el display de 7 segmentos.
4. Ajusta la temperatura ambiente para observar cómo cambia la velocidad del ventilador.

## Notas Adicionales

- El código utiliza una técnica de multiplexación para alternar entre los displays de decenas y unidades.
- El código incluye mecanismos de rebote para evitar la detección de múltiples pulsaciones de botón y garantizar un funcionamiento suave.
- Puedes ajustar los valores TEMPERATURE_MIN y TEMPERATURE_MAX para adaptar el rango de temperatura a tus necesidades específicas.
- El valor de la temperatura en celsius que se muestra en los display esta en un rango de 0 a 99.

## Link al proyecto
https://www.tinkercad.com/things/jI6ACbfG410-ppsegundaparte2/editel



