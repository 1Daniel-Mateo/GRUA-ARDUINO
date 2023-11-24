# GRUA-ARDUINO

La grua arduino es un proyecto en cual nos basamos en varios proyectos arduino para crearlo

### Codigo

1. En arduino IDE  debes de instalar la libreria Serve para poder trabajar con los servomotores y los incluimos.
2. Definimos las variables apartir de incluir la anterior libreria antes mensionada y tambien los ejes que estaran asignados a 90 grados, que cuando utilizemos el joystick estos se muevan a 180 grados.
   
![image](https://github.com/1Daniel-Mateo/GRUA-ARDUINO/assets/126428837/644a2dea-82a1-4231-9be9-bab23ab98e36)

3. Luego en void setup, primero declaramos los pines donde estan ubicados los servomotores que son el 7 y 6. Y  EN servo1.write podemos utilizarlo llamar a las variables ejes que creamos anteriormente, aun que tambien podemos darle un valor inicial de 90.
   
![image](https://github.com/1Daniel-Mateo/GRUA-ARDUINO/assets/126428837/5a6df4cf-ab22-4e6d-a026-7b04ec62f751)

4. por ultimo en void loop, dentro de este creamos 4 condicionales en las cuales en la primera condicion del servo 1 dice que si el valor del pin analogico es menor a 200 y el eje no llego a 180 grados como posicion final, dentro de la codicion en eje1++;
le sumariamos 1 y se sobre pasa el limite usando la varible servo1.write(eje1) no le permitiria pasar.

![image](https://github.com/1Daniel-Mateo/GRUA-ARDUINO/assets/126428837/1387984e-9e7f-4abd-a951-ae3e57155ea8)

5. la siguiente condicion pasa su valor de pasa al cotrario si el el motor no llega al valor de cero entonces y le restara una 1.
   
![image](https://github.com/1Daniel-Mateo/GRUA-ARDUINO/assets/126428837/b34d194d-5699-4842-8f91-b06a7ff3c3c9)

6. Esta mis logica se le aplica al segundo servomotor y por ultimo ponemos un delay para reducir el tiempo en 15 milisegundos los cuales utilizamos para que se puede procesar bien el programa.

![image](https://github.com/1Daniel-Mateo/GRUA-ARDUINO/assets/126428837/e0b0726f-f40e-4857-9af0-a0713b69cc4b)



