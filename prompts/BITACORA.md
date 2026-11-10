# Bitacora de prompts
 
Laboratorio 06: Fundamentos de Ingenieria de Prompts.
 
Herramienta de IA usada: (escribe aqui cual usaste)
 
## Ejercicio 2: Tokens y ventana de contexto

| Texto | Caracteres | Tokens |
|-------|:------------:|:--------:|
| Los estudiantes programan en Java. |7 | 34|
| The students program in Java. |6 |29 |
| desafortunadamente | 4| 18|

- Resultados de los ejercicios 4 y 5: Al iniciar un nuevo chat sí recordo la conversación puesto que tenía la memoria entre chats activada.  
## Ejercicio 3: Temperatura

| Temperatura | % de BiblioTec | Nombres en los 5 intentos |
|:-------------:|:----------------:|:---------------------------:|
| 0 | 100.0%| BiblioTec, BiblioTec, BiblioTec, BiblioTec, BiblioTec|
| 0.5 | 65.3%|BiblioTec, BiblioTec, LibroYa, BiblioTec, LibroYa |
| 1 | 44.5% |PrestaLibro, LibroYa, BiblioTec, PaginaLibre, LectoGo |
| 1.8 |32.2% |LibroYa, NubeDeTinta, BiblioTec, LibroYa, PaginaLibre |

Al subir la temperatura la distribución de probabilidades de los nombres varía, distribuyendo el valor del nombre con mayor porcentaje a sus congéneres. Además, no se muestran nombres diferentes a las opciones ya que ya han sido condicionadas. 
## Ejercicio 4: Prompt vago vs estructurado
 | Criterio | Prompt vago | Prompt estructurado |
|----------|:-------------:|:---------------------:|
| Menciona el objetivo del sistema |Sí |Sí |
| Menciona a los usuarios principales |No |Sí |
| Tiene exactamente 3 funcionalidades |No |Sí |
| Esta en 3 parrafos |No |Sí |
| Lo usaria en un informe real |Sí |Sí |

## Ejercicio 5: Anatomia de un prompt
 | Componente | Texto de mi prompt |
|------------|--------------------|
| Rol |Actua como desarrollador Java. Crea un programa en Java. |
| Instruccion |Actua como desarrollador Java. Crea un programa en Java para gestionar los productos de una tienda usando una clase Producto   con los atributos codigo, nombre, precio y stock. |
| Contexto |Actua como desarrollador Java. Crea un programa en Java para gestionar los productos de una tienda. |
| Ejemplo |Actua como desarrollador Java. Crea un programa en Java para gestionar los productos de una tienda usando una clase Producto   con los atributos codigo, nombre, precio y stock. Usa este estilo para los metodos: getPrecio(), setPrecio(double precio). |
| Formato |Actua como desarrollador Java. Crea un programa en Java para gestionar los productos de una tienda usando una clase Producto   con los atributos codigo, nombre, precio y stock. Usa este estilo para los metodos: getPrecio(), setPrecio(double precio). Explica primero la estructura de la clase y luego presenta el codigo Java. |

