# Sistema de incendio con Arduino
![image](https://github.com/eliascharadia/Sistema-incendio-parcial/assets/89148679/e4026476-55a7-41ea-808f-dd3d3208685e)

# Integrante

- Charadía Elías - 1B

## Descripción
Este proyecto simula un posible alarma contra incendio, utilizando diferentes componentes.
- LCD 16x2:
  Se informa por pantalla la estacion del año y la temperatura actual, medida con el sensor de temperatura TMP36.
  Este componente, para trabajarlo en arduino, se hace uso de su propia libreria "<LiquidCrystal.h>"
- Control con sensor infrarojo:
  Este componente se utiliza de una forma muy basico. Con el boton rojo se puede controlar el encendido y apagado del LCD, y con el boton de
  pausa se puede pausar el sistema contra incendio, colocando al motor en 0 grados y apagando las leds rojas.
  Al igual que el lcd, el control remoto tiene su propia libreria, que fue utilizada.
- Servo motor:
  Cuando haya un posible incendio el servo motor simulara el movimiento de por ejemplo un aspersor, desplazandose en un determinado rango de angulo.
- LEDs:
  Al igual que el servo motor se activan al momento de un incendio haciendo una señal visual alternando el encendido y apagado.
  
El funcionamiento es muy sencillo, cuando el sensor de temperatura detecte temperaturas entre -1 grados y 32 grados, se va a indicar en el display la temperatura actual y la estacion
del año. Cuando detecte una temperatura mayor a 60 grados se activa el sistema de alarma de incendio utilizando todos los componentes anteriormente descritos.
