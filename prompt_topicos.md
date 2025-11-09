TAREA  
Clasificá el siguiente reclamo municipal en EXACTAMENTE UNA de las 10 categorías predefinidas.  

CATEGORÍAS  
1 — Alumbrado público — Luminarias apagadas, rotas o con poca luz en calles, plazas o avenidas.  
2 — Calles y veredas — Baches, roturas de calzada, hundimientos o veredas levantadas.  
3 — Limpieza y residuos — Contenedores desbordados, basura acumulada o falta de recolección.  
4 — Arbolado y espacios verdes — Poda, ramas peligrosas, árboles caídos o mantenimiento de plazas.  
5 — Pluviales e inundaciones — Sumideros tapados, desbordes o acumulación de agua.  
6 — Señalización y tránsito — Semáforos rotos, falta de carteles o problemas de estacionamiento.  
7 — Ruidos molestos — Obras, locales o eventos que generan ruidos fuera de horario.  
8 — Animales y zoonosis — Perros sueltos, mordeduras o animales abandonados.  
9 — Obras y construcciones — Obras sin permiso, escombros en vereda o molestias por construcciones.  
10 — Atención municipal — Quejas por demoras, mal trato o falta de respuesta.  

INSTRUCCIONES  
- Leé SOLO el texto entre <input>…</input>.  
- Determiná la categoría más adecuada según el contenido principal del reclamo.  
- Si hay varios temas, elegí el más relevante.  
- Devolvé **únicamente un JSON válido** con las claves exactas:  
  {"categoria": "<nombre de la categoría>", "descripcion": "<descripción de la categoría>"}  
- Sin texto adicional, sin explicaciones, sin formato de bloque de código.  

EJEMPLOS  
<input>La luz de la esquina de mi casa no funciona desde hace una semana.</input>  
Salida: {"categoria": "Alumbrado público", "descripcion": "Luminarias apagadas, rotas o con poca luz en calles, plazas o avenidas."}  

<input>El contenedor de basura está lleno y nadie lo vacía hace días.</input>  
Salida: {"categoria": "Limpieza y residuos", "descripcion": "Contenedores desbordados, basura acumulada o falta de recolección."}  

TEXTO A CLASIFICAR  
<input>
{{ $json.asunto }}
{{ $json.cuerpo }}
</input>
