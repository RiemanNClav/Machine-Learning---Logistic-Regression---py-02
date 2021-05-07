# Machine-Learning---Logistic-Regression---py-02
application of supervised algorithm
REGRESIÓN LOGISTICA PARA PREDICCIÓNES BANCARIAS
Información del conjunto de datos:

Los datos están relacionados con las campañas de marketing directo de una institución bancaria portuguesa. Las campañas de marketing se basaban en llamadas telefónicas. A menudo, se requería más de un contacto con el mismo cliente, para acceder a si el producto (depósito bancario a plazo) sería ('sí') o no ('no') suscrito.

El objetivo de la clasificación es predecir si el cliente suscribirá (sí/no) un depósito a plazo (variable y).

Información de atributos:
Variables de entrada:

Datos del cliente del banco:
edad (numérico)
trabajo : tipo de trabajo (categórico: "administrativo", "obrero", "empresario", "empleado doméstico", "directivo", "jubilado", "autónomo", "servicios", "estudiante", "técnico", "desempleado", "desconocido")
estado civil: estado civil (categórico: "divorciado", "casado", "soltero", "desconocido"; nota: "divorciado" significa divorciado o viudo)
educación (categórica: "básica.4 años", "básica.6 años", "básica.9 años", "bachillerato", "analfabeto", "curso profesional", "título universitario", "desconocido")
impago: ¿tiene el crédito en mora? (categórico: 'no','sí','desconocido')
vivienda: ¿tiene crédito para la vivienda? (categórico: "no", "sí", "desconocido")
préstamo: ¿tiene un préstamo personal? (categórico: "no", "sí", "desconocido") ## relacionado con el último contacto de la campaña actual:
contacto: tipo de comunicación del contacto (categórico: 'celular','teléfono')
mes: mes del año del último contacto (categórico: 'ene', 'feb', 'mar', ..., 'nov', 'dec')
day_of_week: día de la semana del último contacto (categórico: 'mon','tue','wed','thu','fri')
duración: duración del último contacto, en segundos (numérico). Nota importante: este atributo afecta en gran medida al objetivo de salida (por ejemplo, si la duración=0 entonces y='no'). Sin embargo, la duración no se conoce antes de realizar una llamada. Además, después de la finalización de la llamada y es obviamente conocido. Por lo tanto, esta entrada sólo debería incluirse con fines de referencia y debería descartarse si la intención es tener un modelo de predicción realista. ## Otros atributos:
campaña: número de contactos realizados durante esta campaña y para este cliente (numérico, incluye el último contacto)
pdays: número de días transcurridos desde que el cliente fue contactado por última vez en una campaña anterior (numérico; 999 significa que el cliente no fue contactado previamente)
anterior: número de contactos realizados antes de esta campaña y para este cliente (numérico)
resultado: resultado de la campaña de marketing anterior (categórico: "fracaso", "inexistente", "éxito") ## atributos del contexto social y económico
emp.var.rate: tasa de variación del empleo - indicador trimestral (numérico)
cons.price.idx: índice de precios al consumo - indicador mensual (numérico)
cons.conf.idx: índice de confianza del consumidor - indicador mensual (numérico)
euribor3m: índice euribor a 3 meses - indicador diario (numérico)
nr.employed: número de empleados - indicador trimestral (numérico)
Variable de salida (objetivo deseado):

y: ¿ha suscrito el cliente un depósito a plazo? (binario: "sí", "no")
