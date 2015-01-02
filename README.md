Domotica-Raspberry-Arduino
==========================
Este es un proyecto personal, que ojalá le pueda servir a alguien para aprender o reutilizar.

Se trata de domotizar una casa poco a poco, a un bajo coste y con el menor impacto sobre la casa.

Partes a controlar.
  -Calefacción.
  -Luces.
  -Control del gasto eléctrico.
  -Registro de visitas.
  -Jardinería.
  -Seguridad.
  
  Control.
  El control de sensores y dispositivos lo tendrá la placa Arduino que enviara esa información a la placa Raspberry Pi, esta almacenará los datos en base datos para ser utilizados posteriormente. La raspberry tendrá una interface web para poder controlar todo. Esta instalación se hará en el cuadro de comunicaciones de la casa, para poder tener acceso a todas las partes de la casa con más facilidad.
  El cuadro de comunicaciones tiene alimentacion a 220v y se llevará un cable de red para conectar la Raspberry a la red local y a internet.
  
  Calefaccion.
  La calefacción de mi casa está controlada por un termostato de 2 hilos en el salón.
  Se va a usar la instalción de telefono fijo de casa para mandar información de temperatura de las habitaciones al cuadro de comunicaciones, usando el par de hilos telefónico ya instalado que ahora mismo no se utiliza, para ello he elegido el sensor DS18S20 en modo parasito, para solo usar 2 hilos. Ira montado dentro de un multiplicador de entradas de telefono, se adjunta foto (Próximamente).
  Los sensores envían la información a Arduino y este a Raspberry Pi.
  En el termostato del salón se pondrá en paralelo un relé para activar o desactivar la caldera y permitiendo igualmente el uso del termostato para encender la calefacción, esté relé que funciona a 5v irá conectado mediante un cable de 3 hilos al arduino.
