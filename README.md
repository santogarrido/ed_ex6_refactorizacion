# Issue de tipo Blocker (1)
##### java:S1219
Para poder eliminar esta issue debemos eliminar en el siwtch, en el case 7  lo siguiente 
```label {}``` lo que hay dentro del label si se deja , para que queda tal que así:

```case 7: resultado = "Notable"; break;```
Sin el label

---
# Issue de tipo High (2)
##### java:S3776 
Para esta issue lo que debemos hacer es ir modularizando, dividir en varios métodos el if else para reducir la complejidad cognitiva

```
if (nota >= 0) {
	aprobadoOsuspenso(resultado, ra, nota);
}
```
Hemos metido todos los if else que había y en el método volvemos a hacer otro método para seguir modularizando

```
else {
    tipoSuspenso(resultado, ra, nota);
}
```

##### java:S115 
Para poder eliminar esta issue debemos crear una constante con el valor ```Nota para```.

Para ello creamos lo siguiente ```private static final String NOTA_PARA = "Nota para"``` y sustituir donde estén los ```Nota para``` por nuestra constante

---
# Issue de tipo Medium (12)
##### java:S106 (7)
Para esta issue debemos de crear un objeto ```Logger()``` y reemplazarlo por los ```System.out.println()```

##### 