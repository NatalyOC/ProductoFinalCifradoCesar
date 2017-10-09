# Producto Final
## Cifrado César
>Crea una web que pida, por medio de un prompt(), una frase al usuario y devuelva el mismo mensaje encriptado según el algoritmo de Cifrado César con el parámetro de desplazamiento de 33 espacios hacia la derecha.

*Diagrama de Flujo
*Pseudocodigo

####Pseudocodigo:
~~~
Proceso Cifrado Cesar
         Hacer 
	Escribir "Menu"
	Escribir "1. Cifrar"
	Escribir "2.- Descifrar"
	Segun strMenu Hacer
		1:
			Escribir "Ingrese texto a Cifrar"
			Leer text
			SubProceso encrypt <- cipher ( text)
				Para i<-0 hasta text.length cada i++
					x<-text.charCodeAt(i)
					code<-code=(x-65+33)%26+65  
					encrypt<-String.fromCharCode(code)+encrypt
				FinPara
				Escribir encrypt
			Fin SubProceso
			
		2:
			Escribir "Ingrese texto a Descifrar"
			Leer text
			SubProceso decoded <- decipher ( text )
				Para i<-0 hasta text.length con i++
					x<-text.charCodeAt(i)
					code<-code=(x+65-33)%26+65  
					encrypt<-String.fromCharCode(code)+encrypt
				FinPara
				Escribir encrypt
			Fin SubProceso
	FinSegun
   Mientras strMenu ¡==3
FinProceso
  
~~~
