# BEDU-Proyecto: Desempeño de estudiantes.
Repositorio para el proyecto final, Módulo Programación y manipulación de datos en R
Dataset proveniente de: [https://archive.ics.uci.edu/dataset/320/student+performance]

El presente proyecto tiene los siguientes objetivos: 
1. Realizar un análisis estadístico de los datos de estudiantes: edad, género, calificaciones, entre otros.
2. Realizar una prueba de hipótesis de comparación de medias para determinar si existen diferencias significativas entre estudiantes por género y de acuerdo con las pruebas presentadas.
##Antecedentes


##Análisis: Media de edad por género, porcentaje de género, media de calificaciones: matemáticas, portugués, matemáticas hombres, portugués hombres, matemáticas mujeres, portugués mujeres.

#Importar datos
d1 <- read.csv(file.choose()) #BD Matemáticas
print(d1) #Visualización

d2 <- read.csv(file.choose()) #BD Portugés
print(d2)

d3=merge(d1,d2,by=c("school","sex","age","address","famsize","Pstatus","Medu","Fedu","Mjob","Fjob","reason","nursery","internet"))
print(nrow(d3)) #Unión BD Matemáticas y Portugés

##Prueba de Hipótesis: 

##Conclusiones: estadísticos, el resultado de la prueba.
