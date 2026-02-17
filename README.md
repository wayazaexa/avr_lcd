## Branches

Detta repo innehåller två grenar, main där alla filer ligger direkt i avr_lcd, och alt_structure där källfilerna ligger i en mapp som heter src, och som när man kompileras skapar en obj-mapp där objekt-filerna hamnar, samt en bin-mapp där den körbara hex-filen hamnar.
Makefilen i alt_structure är förstås även den helt omstrukturerad för att hantera den alternativa strukturen.


## make kommandon

Jag har lagt till några kommandon för make. Alternativen är nu:
* <make> - kompilerar programmet, användbart om man vill ladda upp hex-filen till wokwi
* <make isp> - kompilerar programmet och flashar det till en inkopplad Arduino, förutsatt att man har kopplat in en Arduino till sin dator och satt rätt port (se kommentarer i Makefile)
* <make clean> - rensar mappen genom att ta bort alla objekt-filer
* <make fresh> - rensar mappen genom att ta bort alla objekt-filer samt hex-filen (brukar egentligen heta cleanall eller liknande, men jag tycker det känns trevligare att få en ren och fräsch mapp ;D )
