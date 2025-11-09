Tu tarea es extraer una dirección dentro de la Ciudad Autónoma de Buenos Aires (CABA), Argentina, junto con el DNI si estuviera presente en el texto, y generar una resumen objetiva y neutral del reclamo (sin opiniones, juicios de valor ni expresiones de urgencia).

INSTRUCCIONES ESTRICTAS:
- Analizá el texto completo y devolvé solo un JSON válido en una sola línea, con la estructura exacta:
  {"direccion": "<calle y número, ciudad, provincia/estado, país>", "dni": "<DNI o null>", "resumen": "<resumen objetiva del reclamo>"}
- La resumen debe ser una reformulación clara y concisa del reclamo, sin copiar frases textuales ni incluir expresiones emocionales, de molestia, agradecimiento o urgencia.
- No incluir direcciones, DNI, nombres propios ni datos personales dentro de la resumen.
- Si hay varias direcciones, elegí la más precisa (la que tenga número).
- Si no hay dirección válida en CABA, devolvé "direccion": null.
- Si no hay DNI en el texto, devolvé "dni": null.
- No incluyas explicaciones, texto adicional ni formato distinto al JSON.
- La salida debe ser siempre una sola línea JSON válida.

ÁMBITO GEOGRÁFICO:
Solo considerar direcciones dentro de la Ciudad Autónoma de Buenos Aires (CABA), Argentina.

TEXTO:
<input>
{{ $json.asunto }}
{{ $json.cuerpo }}
</input>
