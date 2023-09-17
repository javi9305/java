RESTAURANDO VISUAL STUDIO CODE A VALORES DE FÁBRICA
Omar Ismael
omar_238
Y ¿cómo se logra esto?
1.- Desinstalamos totalmente Visual Studio Code
2.- Abrir la ventana de ejecutar (Tecla [Win] + [R]) Y escribimos:
%userprofile%\AppData\Roaming
Buscamos la carpeta **Code **y nos disponemos a borrarla, seleccionándola y presionando la tecla [Supr]. Esto borrará cualquier configuración previa.
3.- (Opcional) Si tampoco nos interesan conservar las extensiones instaladas previamente se puede optar por borrar también la siguiente carpeta: Otra vez, abrimos la ventana de ejecutar y escribimos:
%userprofile%
En esta carpeta buscamos la que se llame .vscode y la borramos.
4.- Finalmente volvemos a reinstalar VS Code como si fuera la primera vez, y… listo!