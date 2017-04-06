# Gestió de volums Lògics

####    -Descripció del que són:
 Logical Volume Manager es una implementación de un administrador de volúmenes lógicos para el kernel Linux. Se escribió originalmente en 1998 por Heinz Mauelshagen, que se basó en el administrador de volúmenes de Veritas usado en sistemas HP-UX.
####     -Què volen dir les sigles, definició, analogies i exemples de comandes (explicant què fan) vistes a classe de:
####         -PV
Volúmenes físicos (PV): Son las particiones del disco duro con sistema de archivos LVM. 
####         -VG
Grupos de volúmenes (VG): es la parte superior de la LVM. Es la "caja" en la que tenemos nuestros volúmenes lógicos (LV) y nuestros volúmenes físicos (PV). Se puede ver como una unidad administrativa en la que se engloban nuestros recursos. Hay que hacer notar que mientras un PV no se añada al VG, no podemos comenzar a usarlo.

####         -LV
Volúmenes lógicos (LV): es el equivalente a una partición en un sistema tradicional. El LV es visible como un dispositivo estándar de bloques, por lo que puede contener un sistema de archivos (por ejemplo /home)

####     -Entorn de pràctiques: Explicar com farem la pràctica detalladament (màquina virtual i afegir tres discs de 200M)  
Lo que haremos será abrir el virt-manager para crear la maquina virtual y despues en los detalles virtuales de hardware, que entramos allí clicando la bombilla que hay en la parte de arriba y luego clicamos Add Hardware y en Storage ponemos el tamaño que queremos que tenga el dico y en Bus type ponemos la opcion VirtIO, luego finish y hacer el mismo proceso 2 veces mas para acabar agregando los tres discos de 200M.
![Sin titulo](1.png)
####     -Pràctica 1: Creació d'un volum lògic a partir d'un dels tres discs durs (vda per exemple). Aquest volum lògic ha de ser del total de capacitat del disc. El volum de grup s'ha de dir practica1 i el volum lògic dades.
####     -Pràctica 2: Creació d'un sistema de fitxers xfs al volum lògic creat i muntatge a /mnt. També s'ha de crear un fitxer amb dd de 180MB.
####     -Pràctica 3: Creació d'un RAID 1 als dos discos sobrants (vdb i vdc per exemple).
####     -Pràctica 4: Ampliació del volum lògic de dades al raid.
####     -Pràctica 5: Ampliació del sistema de fitxers xfs al tamany actual del volum lògic dades (s'ha de poder fer sense desmuntar-lo de /mnt ja que és xfs). Una vegada creat crearem un nou fitxer de 180M.
