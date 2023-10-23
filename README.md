# Control de Velocidad de un Ventilador

Este código controla un ventilador y ajusta su velocidad según diferentes modos de operación seleccionados a través de botones. La velocidad actual se muestra en dos displays de 7 segmentos para que el usuario pueda ver el estado (velocidad) del ventilador.

![image](https://github.com/Luanda-Toledo/PP_SPD/assets/58377353/2c093748-8f7d-472f-b4f8-7df9ab35ad6f)

## Requisitos de Hardware

- Placa Arduino (se ha probado en Arduino Uno)
- Dos displays de 7 segmentos comunes ánodo (para mostrar la velocidad)
- Cables y protoboard para la conexión
- Un interruptor
- Sensor de temperatura (analógico)
- Motor CC
- Pila de 9V
- Transistor (por ejemplo, NPN como el 2N2222)
- Fotorresistor (LDR - Light Dependent Resistor)
- Resistencias de 10kΩ
  
## Conexiones

- Conecta los displays de 7 segmentos a los pines A4 (UNIDAD) y A5 (DECENA) de la placa Arduino.
- Conecta los segmentos de los displays a los pines 7 (C), 8 (D), 9 (E), 10 (G), 11 (F), 12 (A), y 13 (B) de la placa Arduino.
- Conecta un botón a los pines 4 (BOTON_FIJO), 5 (BOTON_TEMPERATURA) y 6 (BOTON_LUZ) de la placa Arduino. Utiliza resistencias pull-up (10kΩ) para los pines de entrada de los botones.
- Conecta el interruptor o pulsador al pin ENTRADA_INTERRUPTOR. Utiliza resistencias pull-up (10kΩ).
- Conecta el motor CC a la placa Arduino utilizando un transistor NPN (como el 2N2222) para controlar la velocidad.
- Conecta el sensor de temperatura al pin SENSOR_TEMPERATURA y el fotorresistor al pin FOTORRESISTOR utilizando una resistencia de 10kΩ en serie.
- Alimenta la placa Arduino con una pila de 9V o una fuente de alimentación adecuada.

## Uso

1. Cargue el código en su Arduino utilizando el IDE de Arduino.
2. Conecte los componentes siguiendo las conexiones descritas anteriormente.
3. Encienda el interruptor para activar el sistema. El ventilador comenzará a funcionar y la velocidad se mostrará en el display de 7 segmentos.
4. Seleccione el modo de operación utilizando los botones: Modo Fijo, Modo Temperatura o Modo Luz.
5. En el Modo Fijo, el ventilador funcionará a una velocidad fija del 50%. En el Modo Temperatura, la velocidad se ajusta según la lectura del sensor de temperatura. En el Modo Luz, la velocidad se ajusta según la lectura del fotorresistor.
6. Ajuste los valores de TEMPERATURE_MIN, TEMPERATURE_MAX, ANALOG_MIN, ANALOG_MAX, ANALOG_MIN_LUZ y ANALOG_MAX_LUZ según sus necesidades.

## Notas Adicionales

- El código utiliza una técnica de multiplexación para alternar entre los displays de decenas y unidades.
- El código incluye mecanismos de rebote en los botones para evitar la detección de múltiples pulsaciones y garantizar un funcionamiento suave.
- Asegúrese de calibrar adecuadamente los sensores de temperatura y luz para obtener lecturas precisas.
- Los valores de velocidad del motor y número a mostrar en los displays se calculan mediante mapeo de los valores leídos por los sensores.
- El código permite apagar el ventilador al cambiar el interruptor a la posición de apagado.

## Aplicaciones Prácticas 

Este proyecto de control de velocidad de ventilador tiene diversas aplicaciones en situaciones de la vida real:

- **Sistemas de Ventilación Doméstica**: Puede utilizarse para ajustar automáticamente la velocidad de los ventiladores en sistemas de ventilación de casas y apartamentos, garantizando una circulación de aire óptima según las condiciones.

- **Control de Temperatura en Invernaderos**: En entornos agrícolas, el proyecto puede aplicarse para regular la temperatura en invernaderos, lo que es esencial para el crecimiento de plantas sensibles a la temperatura.

- **Sistemas de Refrigeración de Servidores**: En centros de datos y entornos de servidores, se puede utilizar para controlar la velocidad de los ventiladores y mantener las temperaturas dentro de los límites operativos seguros.

- **Ventilación en Automatización Industrial**: En la automatización industrial, el proyecto puede controlar la velocidad de los ventiladores utilizados en sistemas de refrigeración y ventilación en entornos de producción.

- **Proyectos de Internet de las Cosas (IoT)**: Puede ser un componente esencial en proyectos de IoT relacionados con el control del clima, donde se requiere la regulación de la velocidad del ventilador.

Estos son solo algunos ejemplos, y las aplicaciones son variadas. Las posibilidades son amplias, y el código puede adaptarse y personalizarse para satisfacer necesidades específicas en diversas situaciones de aplicaciones prácticas.

## Link al proyecto
https://www.tinkercad.com/things/f52H9MydDr2-ppterceraparte



