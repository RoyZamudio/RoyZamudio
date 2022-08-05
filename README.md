*Instruciones para el uso de las bibliotecas de la actividad I7* Windows 10 Powershell 11


&nbsp;
**Bibiloteca estática "ftrig"**

&nbsp;
1. Después de clonar el repositorio en VS, abrir la terminal.


&nbsp;
2. Ejecutar el siguiente comando en la terminal de VS: g++ main.cc -o app\testlib -I .\lib\include -L .\lib\static -lftrig

&nbsp;
3. Después, ejecutar este otro comando: ./app/testlib.exe


&nbsp;
4. El programa se ejecutará y le pedirá al usuario un número, del cuál será calculado las funciones trignométricas.


&nbsp;
**Nota: Las funciones inversas dan resultados como "nan" en algunos casos ya que funcionan solo con números diferentes a enteros o reales**


&nbsp;
5. Darle enter y en la terminal aparecerá un resultado similar a este:


&nbsp;
Ingrese el valor del cual desea saber su funcion trigonometrica

-3.1

seno(a) = --0.0415808

coseno(b) = -0.999135

tangente(c) = 0.0416167

secante(d) = nan

cosecante(e) = nan

cotangente(f) = -1.25875


&nbsp;
**Bibiloteca dinámica "ftrig"**

&nbsp;
1. Después de clonar el repositorio en VS, abrir la terminal.


&nbsp;
2. Ejecutar el siguiente comando en la terminal de VS: g++ main.cc -o app\testdll -I .\lib\include -L .\lib\dynamic -lftrig


&nbsp;
3. Después, ejecutar este otro comando: .\app\testdll.exe


La salida debería ser igual a la de la biblioteca estática después de que el usuario haya ingresado un número


![d2e345db-ee07-40d8-8a88-f8bda85f22e5](https://user-images.githubusercontent.com/109250047/182996997-689d5de0-ef61-4282-b7e5-e85f22585291.jpg)




Comandos que se usaron para compilar las bibliotecas:


g++ main.cc -o app\testlib -I .\lib\include -L .\lib\static -lftrig


g++ main.cc -o app\testdll -I .\lib\include -L .\lib\dynamic -lftrig





