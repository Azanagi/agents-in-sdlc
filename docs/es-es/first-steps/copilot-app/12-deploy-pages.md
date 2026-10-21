---
title: "Lección 12 - Publica el sitio con GitHub Pages"
description: "Usa la aplicación GitHub Copilot para configurar un flujo de trabajo de Pages, revisar su solicitud de incorporación de cambios y comprobar el Space Quiz publicado."
authors:
  - jamesmontemagno
lastUpdated: 2026-10-12
---

Publica el Space Quiz con GitHub Pages para que tenga un sitio público. Copilot puede preparar el flujo de trabajo y guiar la publicación, pero debes revisar los cambios y confirmar que el sitio está disponible.

En esta lección:

- pedirás a Copilot que configure la publicación con GitHub Pages.
- revisarás el flujo de trabajo y la solicitud de incorporación de cambios antes de fusionarla.
- seguirás la publicación y comprobarás el sitio publicado.

## Escenario

El Space Quiz ya está en un repositorio de GitHub, pero la gente aún necesita una forma sencilla de probarlo. Publicar el sitio de un solo archivo con GitHub Pages lo pone a disposición en una URL pública sin añadir un servidor ni una dependencia de entorno de ejecución.

## Pide a Copilot que publique el sitio

En la sesión de la aplicación Copilot para `space-quiz`, envía este prompt:

```plaintext
Habilita GitHub Pages para este repositorio. Crea un flujo de trabajo de GitHub Actions que compile el sitio web si es necesario y lo publique en GitHub Pages. Añade un README que describa la aplicación y cómo ejecutarla localmente si aún no existe. Crea una solicitud de incorporación de cambios con estos cambios y fusiónala cuando se superen las comprobaciones obligatorias. Supervisa la publicación hasta que se complete correctamente y, después, indica la URL final del sitio web publicado. Si no tienes permiso para habilitar Pages o fusionar, dime exactamente qué debo aprobar o hacer; no indiques que se ha completado correctamente hasta que el sitio esté disponible.
```

![Diagrama de tres etapas: una solicitud de incorporación de cambios de space-quiz fusionada; una ejecución correcta de GitHub Actions llamada Deploy website con los pasos Build website, Upload artifact y Deploy to Pages; y el Space Quiz publicado en yourname.github.io/space-quiz/.](../../../_images/first-steps-app-pages-deploy.svg)

> [!WARNING]
> Este prompt pide al agente que cree y fusione una solicitud de incorporación de cambios y que cambie la configuración de Pages del repositorio. Revisa las diferencias, los permisos de publicación y cualquier solicitud de aprobación de GitHub antes de continuar.

## Revisa el flujo de trabajo y comprueba la publicación

1. Confirma que el README solo se añade si el repositorio aún no tiene uno.
2. Revisa los cambios de la solicitud de incorporación de cambios, incluidos los pasos de compilación y publicación del flujo de trabajo.
3. Fusiona solo después de que se superen las comprobaciones obligatorias de la solicitud de incorporación de cambios.
4. Sigue la ejecución de publicación de GitHub Actions hasta que se complete correctamente.
5. Abre la URL indicada y confirma que se carga el Space Quiz.

Si el agente no puede habilitar Pages o fusionar la solicitud de incorporación de cambios, sigue las instrucciones concretas que te proporcione. No des la tarea por completada hasta que la publicación finalice correctamente y el sitio esté disponible.

## Resumen y pasos siguientes

El Space Quiz ya está disponible como sitio publicado y has comprobado la publicación en lugar de confiar en el informe del agente. Continúa con la [lección 13: Repaso y pasos siguientes][next-lesson].

[next-lesson]: ../13-review/
