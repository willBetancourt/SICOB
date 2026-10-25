# CU-01 — Enviar mensaje básico por botones

**Actor:** persona sorda o con dificultad del habla.

```mermaid
flowchart TD
  A[Abre panel de frases] --> B[Selecciona una frase]
  B --> C[SICOB recupera el mensaje asociado]
  C --> D[Muestra el texto]
  D --> E[Ofrece reproducir audio]
  E --> F[La persona oyente recibe el mensaje]
```

**Alternativa:** si el audio no está disponible, el texto permanece visible. **Resultado:** mensaje básico presentado.