# Conecta Comunidad

Demo web para presentar un sistema municipal de registro, autorización y seguimiento de necesidades comunitarias.

## Funcionalidades incluidas

- Panel municipal con indicadores y solicitudes recientes.
- Vista de directiva comunitaria.
- Registro de solicitudes con comunidad, categoría, urgencia y ubicación.
- Aprobación y rechazo de directivas.
- Gestión de estados e historial cronológico.
- Mapa territorial demostrativo.
- Filtros, búsqueda y estadísticas.
- Persistencia local en el navegador para la demostración.
- Plantilla de datos preparada para importarse en Google Sheets.

> Todos los nombres, ubicaciones y registros incluidos son ficticios.

## Ejecutar localmente

No requiere instalación ni proceso de compilación. Desde la carpeta del repositorio:

```bash
python -m http.server 4173
```

Luego abre `http://localhost:4173`.

También puede servirse la raíz del repositorio desde cualquier alojamiento de archivos estáticos.

## Estructura

```text
index.html                         Interfaz principal
styles.css                         Diseño responsive
app.js                             Datos demo y lógica funcional
CONECTA_COMUNIDAD_DEMO_DB.xlsx     Plantilla de datos
```

## Alcance técnico actual

Esta entrega es una demo funcional para presentación. Los cambios se guardan en `localStorage` y no se comparten entre dispositivos. El archivo `CONECTA_COMUNIDAD_DEMO_DB.xlsx` contiene las entidades y datos semilla para la siguiente fase de integración con Google Sheets y Google Drive.

La versión operativa multiusuario deberá incorporar autenticación, autorización por alcaldía y un adaptador backend que escriba en Google Sheets o en una base de datos, sin exponer credenciales en el navegador.

## Demo publicada

La versión privada de demostración está disponible en:

https://conecta-comunidad-demo.cristian2200ale.chatgpt.site
