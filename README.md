# Control de horas

Aplicación web para registrar trabajadores, turnos, horas, descuentos y pagos quincenales.

## Publicar actualizaciones

El sitio se publica en GitHub Pages. Cada cambio que se guarde en la rama `main` inicia una publicación automática. La persona que usa la app vuelve a abrir o recarga la misma dirección; no necesita instalar una versión nueva.

URL prevista: https://jsrodelo.github.io/control-de-horas/

## Dónde quedan los registros

Los perfiles, números de cuenta, ajustes y turnos se guardan únicamente en IndexedDB del navegador del dispositivo donde se abre la app. No se envían a GitHub ni se sincronizan con otros dispositivos.

Si se cambia desde el HTML local a la página web, el navegador considera que son ubicaciones diferentes. Para conservar registros existentes, exporta una copia de seguridad desde la app anterior y restáurala una vez en la página publicada. Después, usa siempre la misma dirección y navegador, y descarga copias de seguridad periódicas.

## Privacidad

Este repositorio y la página son públicos. El código fuente del sitio puede verse. Los registros de trabajadores no forman parte de este repositorio; nunca subas archivos JSON de copia de seguridad ni datos reales de trabajadores.

## Publicar desde GitHub

El flujo `.github/workflows/deploy.yml` publica el contenido de la rama `main` con GitHub Actions. GitHub Pages se configura con la fuente **GitHub Actions**. Revisa la pestaña **Actions** para ver el estado de cada publicación.
