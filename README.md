## informacion del sistema operativo

### /proc/cpuinfo - archivo que contiene información del nucleo
informacion completa : less /proc/cpuinfo
<!-- el numero de procesadores no pude ser el qu dice ser, un procesador con 2 nucleos y hyperthreading se reportara como uno de 4 nucleos -->
numeros de procesadores : less /proc/cpuinfo | grep processor | wc -l
<!-- para obtnener el numero exacto de los nucleos, es mejor revisar los id unicos de los nucleos -->
revisando los id de los nucleos: cat /proc/cpuinfo | grep 'core id'
###lscpu
 comando para imprimir detalles de hardware: lscpu
### hardinfo
 herramienta que genera reportes del hardware: hardinfo | less

### lshw
  muestra informacion limitada del cpu: lshw, lshw -class processor

### nproc
  imprime los numeros de procesadores

### dmidecode
### cpuid
### inxi, inxi -C

## kernel
uname -r 


## resources

https://wiki.archlinux.org/

