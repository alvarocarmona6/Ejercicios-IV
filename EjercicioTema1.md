# Álvaro Carmona Oliva

## Ejercicio 1 Consultar en el catálogo de alguna tienda de informática el precio de un ordenador tipo servidor y calcular su coste de amortización a cuatro y siete años. 
Voy a usar [QNAP TVS-882ST3-i7-16G](https://qloudea.com/qnap-tvs-882st3-i7-16g?gclid=CjwKCAjwo4jOBRBmEiwABWNaMSWTd84I-7HuPKFLoH4UqMnd1CRMTKpemFS7PSCQ869zYUzZd1WXdBoCsF0QAvD_BwE)

Su precio con IVA es de 3.023,89 € si le quitamos el IVA quedaría:
3.023,89 € *0,79 = 2.388,87 €
Por tanto para su  amortización a 4 años debemos amortizar cada año al 25 %
	2.388,87 € * 0,25 = 597.21€ cada año 
Para la amortización a 7 años el proceso es algo más detallado:

	Para los dos primeros años (25 %) → 2.388,87 € * 0,25 = 597.21€ x 2 = 1.194,43 € 
	Para tercer y cuarto año ( 15 %) →  2.388,87 € * 0,15 = 358,33 € x 2 = 716,66 €
	Para el quinto año  (10%) → 2.388,87 € * 0,1 = 238,88 € 
	Para el sexto y septimo año (5%) → 2.388,87 * 0.05 = 119.44 € x 2 = 238.88 €
Por último cabe destacar que si sumamos todas las cantidades anteriores tenemos el precio total sin IVA.


## Ejercicio 2 Usando las tablas de precios de servicios de alojamiento en Internet “clásicos”, es decir, que ofrezcan Virtual Private Servers o servidores físicos, y de proveedores de servicios en la nube, comparar el coste durante un año de un ordenador con un procesador estándar (escogerlo de forma que sea el mismo tipo de procesador en los dos vendedores) y con el resto de las características similares (tamaño de disco duro equivalente a transferencia de disco duro) en el caso de que la infraestructura comprada se usa sólo el 1% o el 10% del tiempo.


[Servidor dedicado: ](https://www.hostalia.com/dedicados/?gclid=CjwKCAjwo4jOBRBmEiwABWNaMVUFJZe6YO8shQiYPI_JvG2zLmE2AQH01ZmJoAxtYjlZ9m4SGVdfbBoChyEQAvD_BwE)

[Cloud Server:] (https://www.arsys.es/servidores/cloud?s=cpc&c=315965763&a=19240942683&gclid=CjwKEAjwo4jOBRDmqsavuLfl9CYSJAAFY1oxYoTii-dnyaXpvECf_o18hnbf4Do4h4h358G6gLwG0hoCgK7w_wcB)

Las características de los dos servidores:

Dedicado vs Nube:

Procesador → 2 x Intel® Xeon® E5-2620 v4 (*) vs 8 vCPU Xeon 
RAM → 128 GB vs 16 GB
HD →      2 x 1TB SATA vs 200 GB SSD
Precio → 399,90 €/mes vs 150 €/mes 

El precio anual de cada uno es:
Dedicado = 399,90€   x 12 = 4.798,8 €
Nube = 150 € x 12 = 1800 €

Si lo usáramos un 1 % sería:
Nube = 1800 € x 0,01 = 18 €
Dedicado no se puede usar un 1 %

Si lo usáramos un 10%
Nube = 1800 € x 0,1 = 180 €
Dedicado no se puede usar un 10% 




## Ejercicio 3 En general, cualquier ordenador con menos de 5 o 6 años tendrá estos flags. ¿Qué modelo de procesador es? ¿Qué aparece como salida de esa orden? Si usas una máquina virtual, ¿qué resultado da? ¿Y en una Raspberry Pi o, si tienes acceso, el procesador del móvil?

En mi pc mi procesador es el siguiente: Intel(R) Core(TM) i5-5200U CPU @ 2.20GHz

Mi salida de la orden de flag es la siguiente : 

        alvaro@alvaro-X555LJ:~$ egrep '^flags.*(vmx|svm)' /proc/cpuinfo
        flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx pdpe1gb rdtscp lm constant_tsc arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc aperfmperf eagerfpu pni pclmulqdq dtes64 monitor ds_cpl vmx est tm2 ssse3 sdbg fma cx16 xtpr pdcm pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand lahf_lm abm 3dnowprefetch epb intel_pt tpr_shadow vnmi flexpriority ept vpid fsgsbase tsc_adjust bmi1 avx2 smep bmi2 erms invpcid rdseed adx smap xsaveopt dtherm ida arat pln pts


Al usar una máquina virtual y escribir el comando egrep '^flags.*(vmx|svm)' /proc/cpuinfo no me aparece nada 
el procesador si sale el mismo.



