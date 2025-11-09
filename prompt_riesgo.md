TAREA  
Clasificá el siguiente reclamo municipal según su NIVEL DE RIESGO.  

NIVELES DE RIESGO  
- Bajo — Molestias menores o estéticas sin riesgo para personas ni bienes.  
- Moderado — Afecta parcialmente la seguridad o el funcionamiento, riesgo bajo o medio.  
- Alto — Riesgo concreto para personas o bienes, requiere atención prioritaria.  
- Crítico — Peligro inminente de lesiones graves, incendio o colapso; requiere acción inmediata.  

INSTRUCCIONES  
- Leé SOLO el texto entre <input>…</input>.  
- Evaluá el nivel de riesgo considerando la probabilidad de daño y la gravedad.  
- Devolvé **únicamente el nombre exacto de la categoría de riesgo**:  
  "Bajo", "Moderado", "Alto" o "Crítico".  
- No devuelvas JSON, texto adicional ni explicaciones.  

EJEMPLOS  
<input>Poste inclinado con cables chispeando sobre la vereda.</input>  
Salida: Crítico  

<input>Bache profundo sin señalización en una calle muy transitada.</input>  
Salida: Alto  

<input>Contenedor de basura lleno pero sin olores ni animales.</input>  
Salida: Moderado  

<input>Cartel de calle despintado.</input>  
Salida: Bajo  

TEXTO A CLASIFICAR  
<input>
{{ $json.asunto }}
{{ $json.cuerpo }}
</input>
