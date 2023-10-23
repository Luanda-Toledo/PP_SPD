# Control de Display de 7 Segmentos

Este código está diseñado para controlar un contador de 7 segmentos utilizando una placa Arduino. El contador puede mostrar números en el rango de 0 a 99 y se puede operar mediante botones de suma, resta y reinicio. Además, tiene un interruptor delizante para encender y apagar el sistema.

![image](https://github.com/Luanda-Toledo/PP_SPD/assets/58377353/43071cea-ff1e-4b52-9d88-7da2c8c4ef0a)


## Requisitos de Hardware

	@@ -11,33 +11,37 @@ Este proyecto Arduino implementa un contador de 7 segmentos que muestra un núme
- Tres botones (para suma, resta y reset)
- Resistencias pull-up (10kΩ) para los botones
- Cables y protoboard para la conexión
- Un interruptor o pulsador para alternar entre encencido o apagado.
- 
## Conexiones

- Conecta los displays de 7 segmentos a los pines A4 (UNIDAD) y A5 (DECENA) de la placa Arduino.
- Conecta los segmentos de los displays a los pines 7 (C), 8 (D), 9 (E), 10 (G), 11 (F), 12 (A), y 13 (B) de la placa Arduino.
- Conecta un botón a los pines 3 (ENTRADA_RESTA), 4 (ENTRADA_SUMA) y 5 (ENTRADA_RESET) de la placa Arduino. Utiliza resistencias pull-up (10kΩ) para los pines de entrada de los botones.
- Conecta el interruptor o pulsador al pin ENTRADA_INTERRUPTOR. Utiliza resistencias pull-up (10kΩ).

## Uso

1. Cargue el código en su Arduino utilizando el IDE de Arduino.
2. Conecte los componentes siguiendo las conexiones descritas anteriormente.
3. Utiliza el interruptor o pulsador para alternar entre encendi o apagado.
   - Apagar el sistema.
   - Enecender el contador, puedes utilizar los botones de suma y resta para modificar el contador de dos dígitos. El botón de reset restablecerá el contador a cero.
4. Presione el botón de suma (+) para incrementar el contador.
5. Presione el botón de resta (-) para decrementar el contador.
6. Presione el botón de reset para volver a cero.

## Notas Adicionales

- El código utiliza una técnica de multiplexación para alternar entre los displays de decenas y unidades.
- El contador se reinicia automáticamente a 0 cuando alcanza 99 o se decrementa por debajo de 0.
- Se utiliza una resistencia pull-up interna para los pines de entrada de los botones.
- El código incluye mecanismos de rebote para evitar la detección de múltiples pulsaciones de botón y garantizar un funcionamiento suave.
- Los displays de siete segmentos se utilizan para mostrar el valor actual del contador.

## Link al proyecto
https://www.tinkercad.com/things/gPcymY8TQBo


