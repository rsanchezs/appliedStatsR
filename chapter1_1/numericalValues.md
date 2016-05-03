
# Medidas de posición y dispersión

Las principales medidas de posición y dispersión son la _Media_, obtenida con la función __mean__, la _Mediana_ cuyo valor lo obtenemos con __median__, la _Cuasivarianza_ para la que debemos ejecutar la función __var__; su raíz cuadrada, la _Cuasidesviación típica_, obtenida con __sd__, y los _cuantiles_ que se consiguen con __quantile__.

Un buen resumen de muchas de las medidas de posición se obtiene de una vez con la función __summary__.

<!--sec data-title="Ejemplo 2.2" data-id="ej2_2" ces-->


Se midieron los niveles de colinesterasa en un recuento de eritrocitos de 34 agricultores expuestos a insecticidas agrícolas, obteniéndose los siguientes datos:

10.6, 12.5, 11.1, 9.2, 11.5, 9.9, 11.9, 11.6, 14.9, 12.5, 12.5, 12.5, 12.3, 12.2, 10.8, 16.5, 15, 10.3, 12.4, 9.1, 7.8, 11.3, 12.3, 9.7, 12, 11.8, 12.7, 11.4, 9.3, 8.6, 8.5, 10.1, 12.4, 11.1, 10.2

Las funciones antes mencionadas se aplican a un vector de datos numéricos, por lo que crearemos un vector con los datos de arriba y aplicaremos las funciones antes mencionadas para computar las medidas de posición y dispersión:


```r
> x <- c(10.6, 12.5, 11.1, 9.2, 11.5, 9.9, 11.9, 11.6, 
+        14.9, 12.5, 12.5, 12.5, 12.3, 12.2, 10.8, 16.5, 
+        15, 10.3, 12.4, 9.1, 7.8, 11.3, 12.3, 9.7, 12, 
+        11.8, 12.7, 11.4, 9.3, 8.6, 8.5, 10.1, 12.4, 11.1, 
+        10.2)
> mean(x)
```

```
[1] 11.38571
```

```r
> quantile(x)
```

```
   0%   25%   50%   75%  100% 
 7.80 10.15 11.50 12.40 16.50 
```

```r
> quantile(x, probs = 0.25)
```

```
  25% 
10.15 
```

```r
> var(x)
```

```
[1] 3.448319
```

```r
> sd(x)
```

```
[1] 1.856965
```

```r
> summary(x)
```

```
   Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
   7.80   10.15   11.50   11.39   12.40   16.50 
```
<!--endsec-->
