# Diagrama general de casos de uso — SICOB

Este diagrama reúne los cuatro casos de uso descritos en el documento del proyecto y los tres actores identificados.

```mermaid
flowchart LR
    S[Persona Sorda/Muda] --> U1((Enviar Mensaje Básico por Botones))
    S --> U3((Redactar Mensaje de Texto Libre))
    O[Persona Oyente] --> U2((Seleccionar Frase Básica por Botones))
    A[Administrador de Contenidos] --> U4((Gestionar Frases y Botones Básicos))
    U1 -. <<include>> .-> M((Mostrar Mensaje Básico al Oyente))
    U1 -. <<include>> .-> R1((Reproducir Mensaje Básico en Audio))
    U2 -. <<include>> .-> B((Buscar Video en Lengua de Señas))
    U2 -. <<include>> .-> R2((Reproducir Video en Lengua de Señas))
    U3 -. <<include>> .-> C((Convertir Texto a Voz Artificial))
    U3 -. <<include>> .-> R3((Reproducir Mensaje de Voz al Oyente))
```

## Actores
- Persona Sorda/Muda.
- Persona Oyente.
- Administrador de Contenidos.

**Referencia de origen:** documento SICOB, sección VI, Fig. 9.

## Imagen del diagrama

![Diagrama del caso de uso](./diagrama.svg)
