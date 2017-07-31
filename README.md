- US = Unix System
- Options Commands
	 - many commands have options: `command -letter`
	 - some commands need options be listed before file arguments
	 	- but unix command are designed to pass options first
	 - the fact the no output indicate successfull execution 	 

## Commands
	### Utility
		- to show date: `date` 
		- current users logged in the system: `who` or `who am i`
			- tty, is an ID, that unix gives to each terminal's user
			- sho the date when users logged in
	
	### Echoing characters: 
		- prints an echo: `echo this is a test`
			- a blank line: `echo`
	
	### Files
		- three types on unix
			- ordinary files - whatever file: data, text, programs instructions 
			- directory files - folders
			- special files - typically is some form of I/O
		- a filename not be greater than 255, if it is US just ignores
		- listing files: `ls`
			- to show in one column add option: `-1`
		- display content of a file: `cat <files> `
			- is a short for concatenated
			- pass the files you want to examinate 	 
		- counting number of words: `wc <files>`
			- first is number of lines: `-l`
			- second is number of words: `-w`
			- third is number of characters: `-c`
		- to copy a file: `cp <sourcefile> <destinationfile>`
		- rename a file: `mvi <file> <moveto>`
			- unix not care weather the file exists, it just override it
		- to remove a file: `rm <files>`
			

			
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

## Related
	- c programming language
	- objective-c
	- unix system
	- shell programming
