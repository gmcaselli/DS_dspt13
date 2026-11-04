# Análisis de clientes de restaurantes en EE.UU.

Proyecto del módulo M1 del curso de Data Science (Henry, cohorte DSPT13).
Limpieza y análisis exploratorio de una base de 30.000 clientes de restaurantes
en 10 ciudades de EE.UU., complementada con datos de la API de Yelp.

# Aclaracion:
Se crear una cuenta en Yelp, generar una API key y se guarda en un archivo local Base de datos.txt (no incluido en el repositorio).

## Objetivo

Entender el perfil de los clientes: cuánto gastan, con qué frecuencia visitan,
qué preferencias alimenticias tienen y cómo se relacionan con su ciudad,
estrato socioeconómico, edad e ingresos.

## Contenido del repositorio

| Carpeta | Descripción |

| `Avances-jupyternotebook/` | Notebooks con avances 1, 2 y 3; con la limpieza, el análisis y los gráficos |
| `Documentacion-docs/` | Como se realizaron los notebooks y las conclusiones del análisis |

## Datos

- **Base de clientes:** 30.000 filas y 17 columnas (edad, género, ciudad,
  estrato socioeconómico, frecuencia de visita, gasto promedio, preferencias
  alimenticias, ingresos, etc.). Datos sintéticos.
- **API de Yelp:** 240 restaurantes de Miami (nombre, rating, reseñas, precio, categorías).

## Proceso de limpieza

- Nulos imputados (edad, gasto, preferencias alimenticias).
- Valores fuera de rango corregidos (edades negativas o mayores a 110, frecuencias negativas).
- Teléfonos unificados en formato `+1 (xxx) xxx-xxxx x ext`.
- Eliminación de duplicados y de restaurantes sin precio.

## Principales hallazgos

- Vemos que la mayor cantidad de personas en la ciudad de Miami se inclinan por Mariscos y vegetarianos
Vemos que la mayoría de personas que tienen mas visitas y mas gastan en la ciudad de Miami son los mayores de 66 años.
El estrato socioeconómico que mas se mueve es el Alto y Muy Alto, con el 60% de la muestra. Son los que mas visita tienen y más gastan.

## Cómo ejecutarlo

1. Clonar el repositorio: `git clone https://github.com/gmcaselli/DS_dspt13.git`
2. Instalar las librerías: `pip install pandas numpy matplotlib seaborn requests openpyxl`
3. Abrir los notebooks con Jupyter o VS Code y ejecutar las celdas en orden.
4. Para el notebook de Yelp se necesita una API key propia (ver más abajo).

## Autor

Gerardo Caselli — [GitHub](https://github.com/gmcaselli)
