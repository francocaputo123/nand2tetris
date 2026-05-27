**HDL:** es una manera de designar un nombre para definir *chips* o puertas lógicas.
**Parts:** la lógica programada en el chip, se evalúa dentro de la sección parts.
Hdl *no* es un lenguaje de programación, es un lenguaje *declarativo*.

**Convenciones:**
HDL es case sensitive, por ende, no será lo mismo FOO que foo.
Comentarios: //, /** /

**Buses multibit**
Para declarar una entrada con multiples bit, se declara en las variables de in y out del chip y se hace mediante la sintaxis x[n].

Para obtener variables de salida dentro de los chips, se le asigna el valor a out por ej.
And(a=a, b=b, out=salida1) salida uno almacena el valor de salida de a y b respectivamente, después se podrá usar salida1 como un input de otro chip.

