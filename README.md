# Operations-in-R-
First Quiz

##Visualizar un conjunto de filas/columnas de una base 
x[152:153, ]
x<-hw1_data
x[ ,2]
x[2, ]
x[3, ]
x[1:2, ]
x[48,1]

##Extracción de filas con datos correctos (sin NA)
x<-hw1_data
x[ ,1]
good<-complete.cases(x[ ,1])
good
x[ ,1][good]

##N°de filas con datos correctos 
a<-153
b<-116
a-b

##calculo de datos correctos de una columna
mean(x[ ,1][good])

##Visualización de un conjunto de valores de una subpoblación en específica (Cual es el promedio de radiación solar con Ozone mayor de 31 y temperatura mayor de 40 sin NA(con datos correctos))
x
c<-(x[ ,1]>31)
c
d<-(x[ ,4]>90)
d
e<-(x[ ,2])
g<-c*d*e
g
h<-267+272+203+225+237+188+167+197+183+189
h
i<-h/10
i

#cálculo sobre una subpoblación en especial (Cual fue el promedio de temperatura en el mes de Junio)
five<-(x[ ,5]==6)##fecha
fourth<-(x[ ,4])##temperatura
mean(fourth[32:61])##calculo de la media

#Visualización de un conjunto de valores de una subpoblación en específica sin errores (como estaba el índice la capa de ozono en el mes quinto-Sin errores
three<-(x[ ,5]==5)##fecha
two<-(x[ ,1])##Indice de la capa de ozono
one<-three*two##cálculo para visualización de datos del mes
one##visualización
a<-complete.cases(x[ ,1])##corrección de datos
a##visualización
x[ ,1][a]##extracción de los datos correctos de una subpoblación especial

