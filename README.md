# Others
## Codigo para ejecutar Chrome de forma insegura
chrome.exe --allow-running-insecure-content
## Ejemplo:
"C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" --allow -running -insecure -content  -incognito

## IMAGEN Y ARCHIVOS TXT A PDF

- Requisitos

- Image Magic

[Tutorial](https://www.youtube.com/watch?v=IeUMpoGJ3Jc)

## Converter.bat
~~~
@echo off
Title Conversor de imagenes o archivos txt a PDF
echo ----------------------------------------------------------
echo        En esta carpeta solo debe haber imagenes
echo ----------------------------------------------------------
echo  Tambien convierte el contenido de archivos *.txt en *.pdf
echo ----------------------------------------------------------
pause
convert *.* archivo.pdf
cls
echo -------------------------------
echo Conversion realizada con exito
echo -------------------------------
echo El archivo se llama archivo.pdf
echo -------------------------------
pause
~~~

