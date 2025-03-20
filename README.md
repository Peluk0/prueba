Introducción

Arduino es una plataforma de hardware y software libre ampliamente utilizada en electrónica y robótica educativa. Su versatilidad permite crear proyectos interactivos mediante la integración de componentes como sensores, actuadores y módulos especializados. En este documento, se analizarán tres componentes esenciales: el Prototype Expansion Module, el Sensor Ultrasónico HC-SR04 y el Display de 7 Segmentos 4 Dígitos, explicando sus funciones, conexiones y aplicaciones prácticas.
1. Prototype Expansion Module (1 unidad)
Descripción

El Prototype Expansion Module es una placa de expansión (shield) que se acopla directamente a la placa Arduino (como UNO, Mega o Nano) para facilitar el prototipado de circuitos. Incluye una matriz de protoboard integrada, conexiones organizadas y puertos para sensores y actuadores.
Características Técnicas

    Matriz de protoboard: Permite montar componentes sin necesidad de cables jumper adicionales.

    Puertos etiquetados: Incluye conexiones para alimentación (5V, 3.3V, GND) y pines digitales/analógicos.

    Estabilidad mecánica: Evita desconexiones accidentales al fijarse directamente a la placa Arduino.

Uso Práctico

    Ejemplo de conexión:

        Insertar el shield sobre la placa Arduino.

        Conectar componentes (ej. resistencias, LEDs) directamente en la matriz de protoboard.

Aplicaciones

    Prototipado rápido de circuitos.

    Creación de sistemas embebidos sin soldadura.

2. Sensor Ultrasónico HC-SR04 (1 unidad)
Descripción

Este sensor mide distancias mediante la emisión de ondas ultrasónicas (inaudibles para humanos) y calcula el tiempo que tarda en recibir el eco reflejado. Ideal para proyectos de robótica, seguridad o medición de proximidad.
Características Técnicas

    Rango de medición: 2 cm a 400 cm.

    Precisión: ±3 mm.

    Pines principales:

        Trigger (Trig): Inicia la medición.

        Echo: Recibe la señal reflejada.

Conexión con Arduino

    Conectar VCC a 5V y GND a tierra.

    Trig a un pin digital (ej. D9).

    Echo a otro pin digital (ej. D10).

    Aplicaciones

    Sistemas de estacionamiento asistido.

    Detección de obstáculos en robots.

    Alarma de proximidad.

3. Display de 7 Segmentos 4 Dígitos (1 unidad)
Descripción

Este display muestra números y algunos caracteres usando 7 segmentos LED, con 4 dígitos controlables individualmente. Es común en relojes, contadores o sistemas de medición.
Características Técnicas

    Tipo: Comúnmente cátodo común (CC) o ánodo común (CA).

    Pines:

        Segmentos (A-G y DP): Controlan los LEDs de cada segmento.

        Dígitos (D1-D4): Activan cada uno de los 4 dígitos.

Conexión con Arduino

Para evitar usar demasiados pines, se emplea la técnica de multiplexación:

    Conectar los segmentos (A-G) a pines digitales (ej. D2-D8).

    Conectar los dígitos (D1-D4) a otros pines (ej. D11-D14).

    Usar resistencias de 220Ω en serie con los segmentos.
Aplicaciones

    Temporizadores o cronómetros.

    Visualización de datos de sensores (ej. temperatura, distancia).

Proyecto Integrador

Medidor de Distancia con Display

    Usar el sensor ultrasónico para medir distancia.

    Mostrar el valor en el display de 7 segmentos.

    Montar el circuito en el Prototype Expansion Module para organización.

Componentes Necesarios:

    Arduino UNO.

    Prototype Expansion Module.

    Sensor HC-SR04.

    Display de 7 segmentos 4 dígitos.

    Resistencias y cables.

Conclusión

La combinación de estos componentes permite crear sistemas interactivos complejos de manera accesible. El Prototype Expansion Module simplifica el prototipado, el sensor ultrasónico añade capacidades de medición precisa, y el display ofrece retroalimentación visual. Estos elementos son fundamentales para proyectos educativos, robótica o automatización, demostrando la versatilidad de Arduino como plataforma de desarrollo.
