<!-- la nada -->

---

class: middle

.right-column[
# Pedro Almirall

github.com/ktowen <br>
twitter.com/ktowen_dev <br>
]
.left-column[ .avatar[
        ![Yo](images/yo.jpg)
    ]
]

---

class: hero potter middle

# Django ORM
## y el misterio de las agregaciones multiples

---

![Saludo con guantes, cuidado con el COVID](images/handshake.jpg)

---

class: middle center

![Logo de Django](images/django-logo.png)

---

class: middle center hero

# ORM

---

class: middle center

![Diagrama ORM](images/orm.png)

---

class: middle center

![Modelos de ejemplo](images/modelos.png)

---

class: middle center

![Todos los autores](images/autor-all.png)
![Tabla autores](images/tabla-autores.png)

---

class: middle center

![Todos los libros](images/libro-all.png)
![Tabla libro](images/tabla-libros.png)

---

class: middle center

![Todos los articulos](images/articulo-all.png)
![Tabla articulo](images/tabla-articulos.png)

---

class: middle center

![Consulta de autores anotados con los precios de sus libros](images/annotate-precios.png)
![Tabla de autores anotados con los precios de sus libros](images/tabla-suma-precios.png)

---

class: middle center

![Consulta de autores anotados con el total de articulos](images/annotate-articulos.png)
![Tabla de autores anotados con el total de articulos](images/tabla-total-articulos.png)

---

class: middle center

![Consulta de autores con múltiples anotaciones](images/annotate-multiple.png)
![Tabla de autores con múltiples anotaciones](images/tabla-annotate-no.png)

---

class: middle center

## ¿Entonces, qué pasa?

---

class: middle center

![Consulta de autores con múltiples anotaciones y los nombres](images/annotate-full.png)

---

class: middle center

.max-height-img[![Tabla de autores con múltiples anotaciones y los nombres](images/tabla-full.png)]

---

class: middle center

## No es culpa de Django

---

class: middle center

## No mucho

---

class: middle center

.max-height-img[![Meme traductora](images/meme-traductora.png)]

---

class: middle center

## ¿Cómo solucionarlo?

---

class: middle center

## Subconsultas SQL

---

class: middle center

![Consulta SQL](images/query-referencia.png)

---

class: middle center

## Dímelo en Django

---

class: middle center

## django.db.models.Subquery

---

class: middle center

## TLDR. Se complica

---

class: board

## Tarea:

- Intentar usar Subquery

---

class: middle center

## Mejor vamos a innovar

---

class: middle center

![Django Subquery preparada](images/subquery.png)

---

class: middle center

![Usando annotate con los Subqueries preparados](images/annotate-subquery.png)

---

class: middle center

![Query sql final](images/query-final.png)

---

class: middle center

![Query sql final](images/query-final-selected.png)
---

class: middle center

## Lo que queríamos ver

![Tabla resultado correcto](images/tabla-annotate-ok.png)

---

class: board

## Tarea:

- Comparar los resultados de usar EXPLAIN para todas las consultas

---

class: middle center

![Referencia en la documentación](images/documentacion.png)

.bottom[
    [Combining multiple aggregations](https://docs.djangoproject.com/en/3.1/topics/db/aggregation/#combining-multiple-aggregations)
]

---

class: middle center

![Reporte en el tracker de django](images/issue.png)

.bottom[
    [Multiple table annotation failure](https://code.djangoproject.com/ticket/10060)
]

---

class: middle

## Django ORM y el misterio de las agregaciones multiples

<hr>

.right-column[
# Pedro Almirall

github.com/ktowen <br>
twitter.com/ktowen_dev <br>
]
.left-column[ .avatar[
        ![Yo](images/yo.jpg)
    ]
]
