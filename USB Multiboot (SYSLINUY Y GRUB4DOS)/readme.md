------------------------
Requisitos USB MULTIBOOT
------------------------

XBOOT
Image Magic

-----------------------------------------------------------------------
USB CON VARIOS SISTEMAS OPERATIVOS (SYSLINUX)
-----------------------------------------------------------------------

[Tutorial](https://www.youtube.com/watch?v=pkb0Ijl2Z78)

- Descomprimimos el archivos multiboot.zip tal cual el archivo a nuestra unidad USB
- Copiamos las isos en la carpeta ISOS
- Nos vamos a la carpeta Windows y editamos los archivos con extensión cfg, buscamos lo siguiente:

set MYISO=WIN7_X86-X64.iso

- Cambiamos "WIN7_X86-X64" por el nombre de la iso de nuestro Wiindows 7
- Guardamos

----------------------
Archivo Windowsxp.cfg 
----------------------

map /multiboot/ISOs/WINXP_X86.ISO (0xff)
rewrite (99) [FiraDisk]nStartOptions=cdrom,vmem=find:/multiboot/ISOS/WINXP_X86.ISO;n0

Remplazamos WINXP_X86.ISO por el nombre de nuestra iso.

----------------------------------------------------------------------------------------------------

Arrancar desde el disco duro 

title Boot from Arrancar desde el disco duro
rootnoverify (hd0,0)
chainloader (hd0,0)+1

----------------------------------------------------------------------------------------------------

--------------------------------------------
USB CON VARIOS SISTEMAS OPERATIVOS (SYS4DOS)
--------------------------------------------

[Tutorial](https://www.youtube.com/watch?v=NnhyKfFEyMs)

-Descomprimimos el archivos multiboot.zip tal cual el archivo a nuestra unidad USB
-Copiamos las isos en la carpeta ISOS
-Nos vamos a la carpeta Windows y editamos los archivos con extensión cfg, buscamos lo siguiente:

set MYISO=WIN7_X86-X64.iso

-Cambiamos "WIN7_X86-X64" por el nombre de la iso de nuestro Wiindows 7
-Guardamos

-----------------------------------
Archivo Windowsxp.cfg 
-----------------------------------

map /multiboot/ISOs/WINXP_X86.ISO (0xff)
rewrite (99) [FiraDisk]nStartOptions=cdrom,vmem=find:/multiboot/ISOS/WINXP_X86.ISO;n0

Remplazamos WINXP_X86.ISO por el nombre de nuestra iso.

--------------------------------------------------------------------------

Arrancar desde el disco duro

title Boot from Arrancar desde el disco duro
rootnoverify (hd0,0)
chainloader (hd0,0)+1

---------------------------------------------------------------------------

--------------------------------------------------------------------------------------------------------------------------
                                             IMPORTANTE
--------------------------------------------------------------------------------------------------------------------------

Para meter un sistemas operativo en un pendrive deben usar el programa iso to usb

--------------------------------------------------------------------------------------------------------------------------
                                             CD MULTIBOOT CON EASYBOOT
--------------------------------------------------------------------------------------------------------------------------

[Tutorial](https://www.youtube.com/watch?v=88B3NCw0o4w)
