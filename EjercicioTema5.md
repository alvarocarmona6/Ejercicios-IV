# Álvaro Carmona Oliva


## 1. Instalar los paquetes necesarios para usar KVM. Se pueden seguir estas instrucciones. Ya lo hicimos en el primer tema, pero volver a comprobar si nuestro sistema está preparado para ejecutarlo o hay que conformarse con la paravirtualización.
Lo volvemos a comprobar con el kvm-ok
       ![captura](https://github.com/alvarocarmona6/Ejercicios-IV/blob/master/capturas/tema5-1.png)


## 2. Crear varias máquinas virtuales con algún sistema operativo libre tal como Linux o BSD. Si se quieren distribuciones que ocupen poco espacio con el objetivo principalmente de hacer pruebas se puede usar CoreOS (que sirve como soporte para Docker) GALPon Minino, hecha en Galicia para el mundo, Damn Small Linux, SliTaz (que cabe en 35 megas) y ttylinux (basado en línea de órdenes solo).
Voy a instalar DSL , primero creamos el disco duro con


        qemu-img create -f qcow2 servidor.img 8G

![captura](https://github.com/alvarocarmona6/Ejercicios-IV/blob/master/capturas/captura5-2.png)

y luego el siguiente comando (tenemos que tener la iso de dsl descargada)


        qemu-system-x86_64 -hda servidor.img -cdrom dsl-4.1.rc1.iso    

![captura](https://github.com/alvarocarmona6/Ejercicios-IV/blob/master/capturas/captura5-22.png)


## 5 Crear una máquina virtual ubuntu e instalar en ella alguno de los servicios que estamos usando en el proyecto de la asignatura.
Lo he realizado en mi  [proyecto](https://github.com/alvarocarmona6/ProyectoIV/).


## 6. Instalar una máquina virtual con Linux Mint para el hipervisor que tengas instalado.
Voy a instalar DSL , primero creamos el disco duro con


        qemu-img create -f qcow2 linxmint.img 8G

![captura](https://github.com/alvarocarmona6/Ejercicios-IV/blob/master/capturas/captura6-1.png)

y luego el siguiente comando (tenemos que tener la iso de dsl descargada)


        qemu-system-x86_64 -hda linxmint.img -cdrom linuxmint-18.3-cinnamon-32bit.iso 


![captura](https://github.com/alvarocarmona6/Ejercicios-IV/blob/master/capturas/captura6-22.png)





