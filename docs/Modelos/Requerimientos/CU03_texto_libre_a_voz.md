# CU-03 — Redactar texto libre y reproducir voz

**Actor:** persona sorda o con dificultad del habla.

```mermaid
flowchart TD
  A[Abre módulo de texto libre] --> B[Redacta el mensaje]
  B --> C[Revisa el contenido]
  C --> D{¿Hay síntesis de voz disponible?}
  D -- Sí --> E[Reproduce voz artificial]
  D -- No --> F[Mantiene el texto visible e informa la limitación]
```

**Resultado:** el mensaje queda disponible en texto y, si el dispositivo lo permite, en voz. Este caso de uso no representa traducción automática a LSC.