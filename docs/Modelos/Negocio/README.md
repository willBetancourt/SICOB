# Modelo de negocio SICOB

Los diagramas siguientes representan procesos de comunicación independientes de la solución informática. Son hipótesis iniciales que deben contrastarse con el cliente.

## Proceso 1 — Comunicación básica: persona sorda hacia persona oyente
```mermaid
flowchart TD
  A[Persona sorda identifica el mensaje] --> B[Selecciona o expresa una frase]
  B --> C[Persona oyente recibe el mensaje]
```
**Descripción:** intercambio cotidiano de saludos, presentaciones y expresiones frecuentes.

## Proceso 2 — Comunicación básica: persona oyente hacia persona sorda
```mermaid
flowchart TD
  A[Persona oyente formula una frase] --> B[Transmite el mensaje en una forma comprensible]
  B --> C[Persona sorda recibe e interpreta el mensaje]
```
**Descripción:** comunicación inversa, que puede requerir una representación visual en LSC.

## Proceso 3 — Comunicación compleja
```mermaid
flowchart TD
  A[Persona sorda necesita expresar un mensaje no rutinario] --> B[Formula el mensaje]
  B --> C[Persona oyente recibe e interpreta el contenido]
```
**Descripción:** situaciones que no se resuelven con expresiones predefinidas.

## Proceso 4 — Gestión de contenidos
```mermaid
flowchart TD
  A[Responsable detecta necesidad de actualizar contenido] --> B[Revisa o crea frase/video/parámetro]
  B --> C[Valida el contenido]
  C --> D[Publica versión actualizada]
```
**Descripción:** mantenimiento del catálogo para conservar utilidad y adecuación del contenido.

## Vista general de procesos
```mermaid
flowchart LR
  S[Persona sorda] <--> B[Comunicación básica]
  O[Persona oyente] <--> B
  S <--> C[Comunicación compleja]
  O <--> C
  A[Administrador de contenidos] --> G[Gestión de contenidos]
  G --> B
  G --> C
```
