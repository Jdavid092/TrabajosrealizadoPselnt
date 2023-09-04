# fullcoders-04-09

Algoritmo cargar_notas_alumnos
	Definir notas, nota, promedio, aprobados Como Real
	Definir cantida_alum, cantidad_notas, desprobado Como Real
	Definir condicion Como Cadena
	cantida_alum <- 0
	cantidad_notas <- 1
	aprobados <- 0
	desprobado <- 0
	notas <- 0
	Escribir '¿Presiones s= si o S=si para agregar mas notas al Alumno', cantida_alum, '?'
	Leer condicion
	Mientras (condicion=='s' O condicion=='S') Hacer
		Repetir
			Escribir '¿Ingrese Nota  ', cantidad_notas, ' '
			Leer nota
			notas <- notas+nota
			cantidad_notas <- cantidad_notas+1
		Hasta Que cantidad_notas=3
		promedio <- notas/5
		cantidad_notas <- 0
		Si promedio<6.0 Entonces
			desprobado <- desprobado+1
		SiNo
			aprobados <- aprobados+1
		FinSi
		cantida_alum <- cantida_alum+1
		Escribir '¿Presiones S/s para Agregar mas notas de Alumnos', cantida_alum, '?'
		Leer condicion
	FinMientras
	Escribir 'Cantidad de Alumnos Aprobados', aprobados
	Escribir 'Cantidad de Alumnos Desaprobados', desprobado
FinAlgoritmo
