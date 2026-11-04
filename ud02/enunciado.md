# Práctica 2. Del compromiso a la evidencia

## El encargo

Elena recibe un informe que dice «tenemos procedimientos y hacemos copias».
Quiere saber qué riesgos siguen abiertos y cómo comprobar que se cumplen los
compromisos. Prepara un diseño pequeño de seguimiento del mantenimiento externo.

Usa lo aprendido en [Cumplir no es tener papeles](https://www.apuntesinformaticafp.com/cursos/cumplir_no_es_tener_papeles.html), basándote en la [empresa ficticia Nébula Segura](https://www.apuntesinformaticafp.com/actividades/ndec/caso_nebula_segura.html).
La práctica está dimensionada para unas **dos horas, incluida la revisión**,
aprovechando los «Para hacer». No necesitas instalar herramientas ni entregar UD1
de nuevo. Este expediente es independiente de las soluciones que propusiste allí.

## Expediente de partida

Marta coordina mantenimiento. Iria y su equipo administran sistemas. Nuria guarda
contratos y fechas. Álex revisa cumplimiento y comunica resultados a Elena.
Prisma presta soporte externo. Para este ejercicio analizamos únicamente las
bajas de sus accesos y la recuperación de configuraciones de los servicios privados.

### Compromisos y funcionamiento

- **O1 — Contrato:** retirar los accesos de terceros al finalizar su autorización.
  El alcance incluye todas las cuentas de Prisma y sus subcontratas autorizadas.
- **O2 — Contrato:** mantener copias de las configuraciones administradas y poder
  recuperarlas para restablecer el servicio. No se ha aportado un plazo contractual
  concreto de recuperación.
- **Bajas:** Nuria envía avisos por correo a Iria. Sistemas ejecuta las bajas que
  recibe y deja fecha de ejecución. No existe una revisión periódica que confronte
  todos los vencimientos con las cuentas todavía activas. Hay cambios semanales
  de personal externo; no se ha implantado una baja automática.
- **Copias:** hay tareas nocturnas. Las últimas siete muestran «correcta» y una
  persona revisa esos mensajes. No se ha probado restaurar una configuración ni
  se ha contrastado si las copias incluyen todos los sistemas del alcance.
  Los cambios de configuración son semanales. Una pérdida podría interrumpir
  servicios y exigir reconstrucción manual; no consta una pérdida ya ocurrida.
- **Documentos:** existen `bajas-final.docx` y `bajas-final-2.docx`, sin aprobación
  ni versión identificadas. Los registros de bajas se guardan en una hoja que
  puede editar todo el equipo técnico, sin historial de cambios habilitado.
- **Objetivo interno:** ejecutar a tiempo todas las bajas debidas. Es una meta
  de Nébula para este seguimiento, no un porcentaje impuesto por una norma.

### Datos de revisión: periodo M1

Es un mes ficticio. La revisión se realiza al terminar el día 30. Los registros
aportados cubren **todas las autorizaciones que vencían en M1** dentro del alcance,
incluidas las de subcontratas. Las fechas de ejecución se han contrastado con las
cuentas. No hay otras bajas debidas en este periodo.

| Autorización | Vencimiento | Aviso a sistemas | Ejecución de la baja |
|---|---|---|---|
| A01–A08 (ocho autorizaciones) | Días 2 a 16 | Antes de cada vencimiento | En su fecha de vencimiento |
| A09 | Día 18 | Día 19 | Día 19 |
| A10 | Día 22 | Día 24 | Día 24 |
| A11 | Día 25 | Día 27 | Día 27 |
| A12 | Día 28 | Día 29 | Pendiente; cuenta activa al cierre |

Para el indicador se considera puntual una baja ejecutada, como máximo, en la
fecha de vencimiento. Esta simplificación por días es propia del ejercicio.
No se aportan evidencias de utilización indebida de las cuentas.

### Una organización con consecuencias diferentes

Como contraste, considera una entidad sanitaria ficticia. Tiene la misma
frecuencia de cambios y los mismos fallos de bajas, pero esas cuentas permiten
consultar historias clínicas e interrumpir una aplicación de atención a pacientes.
Es una variante para comparar consecuencias: no es un nuevo cliente confirmado
de Nébula ni exige elaborar otro expediente completo.

## 1. Alcance y fundamento

En **cuatro o cinco líneas**, delimita qué procesos, servicios y terceros incluyes,
qué queda fuera y qué funciones necesitas para revisarlos. Recoge O1 y O2 en la
tabla de obligaciones e indica una recomendación de gestión para cada una.
Distingue la exigencia contractual de tu recomendación interna.

Recupera los apartados 29–32 y 45–47 de la sentencia C-340/21 comentada en la
primera clase. En **dos frases**, explica por qué ni «hubo un incidente» ni
«tenemos medidas» bastan, por sí solos, para concluir si las medidas de seguridad
eran adecuadas. Indica una evidencia pertinente para examinarlas. La sentencia
trata seguridad de datos personales; no certifica el cumplimiento del ENS ni
determina por sí sola el cumplimiento de O1 u O2.

**Pistas:** «Perímetro regulatorio y aplicabilidad» y «Modelo de gestión actualizado».
No se pide una búsqueda jurídica nueva ni un catálogo de normas.

## 2. Dos riesgos y su tratamiento

Analiza **R1, accesos que permanecen activos tras el vencimiento**, y **R2,
imposibilidad de recuperar una configuración cuando se necesita**.

Para cada uno:

- Describe causa, evento, consecuencia y propietario del riesgo.
- Identifica los controles existentes y qué permite afirmar la evidencia disponible.
- Valora el **residual actual** con la escala de los apuntes: P e I de 1 a 3,
  horizonte de doce meses; calcula P × I. Prioridades: 1–2 ordinaria,
  3–4 preferente y 6–9 urgente. Justifica ambos valores con los hechos o con una
  hipótesis explícita. La falta de datos no equivale a riesgo bajo.
- Propón un tratamiento con responsable, recurso y plazo relativo a la revisión.
  Estima el **residual previsto** tras comprobar su eficacia: P, I y producto.
  Explica qué cambiaría y qué prueba necesitarías antes de aceptar esa reducción.

Ordena los dos riesgos y justifica la prioridad. No hay una única puntuación
correcta si la valoración está fundamentada; un empate también necesita decisión.
No presentes tus mejoras como ya implantadas ni aceptes un incumplimiento porque
la puntuación sea baja.

Después compara R1 con la entidad sanitaria: mantén la misma P que hayas usado
para Nébula, reconsidera I, calcula el resultado y explica la diferencia en
**tres o cuatro líneas**. Si ambos impactos son altos, justifica qué consecuencias
distintas quedan ocultas por compartir número.

**Pistas:** «Riesgos de cumplimiento», comparación pyme/sanidad y diferencia entre
riesgo actual y previsto. La escala es didáctica, no una fórmula obligatoria de ISO.

## 3. Documentación que permita comprobar

Completa la matriz con **dos recorridos**, O1–R1 y O2–R2. Para cada uno concreta
el control propuesto, quién ejecuta, quién revisa, cuándo y qué registro permitirá
comprobarlo. Define qué resultado demostraría que el control funciona. No se
pide realizar restauraciones ni retirar cuentas reales.

Prepara un **mapa documental de cuatro filas**: obligaciones, riesgos, procedimiento
y registros de revisión. Pueden ser secciones de un único archivo. Identifica
propietario, aprobación cuando corresponda, versión/fecha, permisos y criterio
de conservación. Explica cómo resolverías los dos «final» y protegerías la
trazabilidad de la hoja de bajas. No inventes un plazo legal de conservación.

**Pistas:** «Documentación, evidencias y trazabilidad»: índice, metadatos, copias
y recorrido obligación–riesgo–control–registro.

## 4. Revisión para Elena

Calcula el porcentaje de bajas puntuales de M1, mostrando numerador y denominador,
y compáralo con el objetivo interno. Explica qué permite concluir y qué no.
Concreta quién calculará el indicador, con qué registros y con qué periodicidad;
indica cómo tratarías un mes sin vencimientos o con datos incompletos.

Redacta un registro breve con **resultado, corrección del caso abierto, acción
para evitar que se repita, responsable, plazo propuesto y comprobación posterior**.
Distingue lo ejecutado según el expediente de lo que propones hacer. No conviertas
un aviso tardío en prueba de acceso indebido.

**Pistas:** indicador de bajas, corrección frente a acción correctora y «Diseño
del sistema de cumplimiento».

## Cómo presentar el trabajo

Copia el contenido del siguiente bloque en `ud02/practica.md`. Las filas vacías
son espacios para completar, no ejemplos de solución. Básicamente para usar archivo
de texto (con formato estructurado con markdown). Así podrás autocorregirlo usando
la rúbrica. Y yo también 😀. 

Puedes reutilizar el trabajo formativo y consultar apuntes, documentación,
Internet e IA, comprendiendo y justificando las decisiones. Declara la ayuda
utilizada; trabaja solo con datos ficticios.

La [rúbrica](rubrica.md) está disponible desde el principio. Puedes intentar
primero la actividad y después usarla para revisar, mejorar y autoevaluarte.
La nota definitiva la pondré tras revisar tu trabajo y te devolveré un informe
en tu repositorio.

Publica tus commits en tu repositorio privado. Cuando quieras presentar, crea
**y publica la etiqueta** `practica-ndec-02-v1` sobre el commit que deba corregir.
Puedes presentar hasta tres versiones antes del plazo, utilizando
`practica-ndec-02-v2` y `practica-ndec-02-v3`, sin mover ni borrar las anteriores.
No adjuntes archivos ni registres de nuevo la URL en Moodle: **la etiqueta
publicada me indica que el trabajo está presentado para corregir**.

## Plantilla para practica.md

```markdown
# Práctica 2. Del compromiso a la evidencia en Nébula Segura

## 1. Alcance y fundamento

Alcance y funciones:

| ID | Obligación y fuente | Recomendación interna |
|---|---|---|
| O1 | | |
| O2 | | |

Interpretación de la sentencia y evidencia pertinente:

## 2. Dos riesgos y su tratamiento

| Riesgo | Causa | Evento | Consecuencia | Propietario | Control existente y límites de su evidencia |
|---|---|---|---|---|---|
| R1 | | | | | |
| R2 | | | | | |

| Riesgo | P actual y motivo | I actual y motivo | P × I y prioridad | Incertidumbre o hipótesis |
|---|---|---|---|---|
| R1 | | | | |
| R2 | | | | |

| Riesgo | Tratamiento propuesto | Responsable, recurso y plazo | P/I/producto previstos | Motivo del cambio y prueba necesaria |
|---|---|---|---|---|
| R1 | | | | |
| R2 | | | | |

Orden de prioridad y justificación:

Contraste de R1 con la entidad sanitaria (P, I, producto y explicación):

## 3. Documentación que permita comprobar

| Obligación y riesgo | Control propuesto | Ejecución y revisión: quién y cuándo | Registro y resultado que demostraría eficacia |
|---|---|---|---|
| O1–R1 | | | |
| O2–R2 | | | |

| Documento o sección | Propietario y aprobación | Versión y fecha propuestas | Consulta, edición y conservación |
|---|---|---|---|
| Obligaciones | | | |
| Riesgos | | | |
| Procedimiento | | | |
| Registros de revisión | | | |

Tratamiento de los dos «final» y de la hoja sin historial:

## 4. Revisión para Elena

- Indicador M1 (operación y resultado):
- Objetivo, interpretación y límites:
- Responsable, registros de origen y periodicidad propuesta:
- Mes sin vencimientos / datos incompletos:

| Resultado observado | Corrección propuesta | Acción para evitar repetición | Responsable y plazo | Comprobación posterior |
|---|---|---|---|---|
| | | | | |

## Revisión antes de presentar

- Riesgos: nivel de referencia y evidencia en mi trabajo:
- Documentación: nivel y evidencia:
- Ayuda y fuentes utilizadas:
```
