# Diario TDD

## Ciclo 1

### Red
- Prueba añadida: test_one_feature_is_tiny()
- Técnica de diseño de pruebas empleada: Al tener una única prueba no se ha usado una técnica en especifico, se coge un valor para comprobar que devuelve bien.
- Motivo de elegir este caso: Solo tenemos que comprobar un único valor
- Fallo observado: La función debería devolver tiny pero no es el caso.

### Green
- Código mínimo escrito: Que la función siempre devuelva tiny independientemente del valor.
- Resultado de las pruebas: Devuelve el tiny, es correcto.

### Refactor
- Mejora realizada, o motivo por el que no era necesaria: No se realiza refactorización en este ciclo.

---

## Ciclo 2

### Red
- Prueba añadida: test_zero_features_is_invalid()
- Técnica de diseño de pruebas empleada: Usamos un diseño en particiones equivalentes para el cual cuando es menor que 1 la prueba espera un ValueError, y cuando no espera "tiny".
- Motivo de elegir este caso: tenemos grupos que trabajan de forma similar y es mas optimo dividir el espacio con caracterícticas similares.
- Fallo observado: La función debería devolver ValueError pero no lo devuelve porque no esta implementado.

### Green
- Código mínimo escrito: Un if en el que de ser menor que 1 el valor, devuelve un ValueError, si no devuelve "tiny".
- Resultado de las pruebas: Al ser menor que 1 devuelve un ValueError.

### Refactor
- Mejora realizada, o motivo por el que no era necesaria: No se realiza refactorización en este ciclo.

---

Copiad este bloque para cada ciclo.
