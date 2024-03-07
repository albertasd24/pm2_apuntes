# PM2: Gestor de Procesos Node.js

## Introducción

[PM2](https://pm2.keymetrics.io/) es un gestor de procesos avanzado para aplicaciones Node.js. Su principal objetivo es facilitar la administración y el despliegue de aplicaciones Node.js en entornos de producción, asegurando la estabilidad y el rendimiento.

## Instalación

Puedes instalar PM2 globalmente utilizando npm:

```bash
npm install pm2 -g
```

## Uso Básico
### Iniciar una aplicación
Para iniciar una aplicación con PM2, simplemente ejecuta el siguiente comando:
```bash
pm2 start app.js
```

### Verificar estado de los procesos
Para ver el estado de los procesos gestionados por PM2:
```bash
pm2 status
```

### Detener una aplicación
Detener una aplicación se realiza con el siguiente comando:
```bash
pm2 stop app.js
```

# Características Principales
1. Auto-reinicio
PM2 monitoriza continuamente las aplicaciones y las reinicia automáticamente en caso de fallos, asegurando así una alta disponibilidad.

2. Escalabilidad
Puedes escalar aplicaciones horizontalmente con PM2, permitiendo ejecutar múltiples instancias de una aplicación para distribuir la carga.
```bash
pm2 scale app.js 4
```
3. Logs y Monitorización
PM2 proporciona un sistema de registro robusto y herramientas de monitorización para evaluar el rendimiento de las aplicaciones.
```bash
pm2 logs
```
4. Configuración
PM2 permite personalizar la configuración de cada aplicación a través de un archivo de configuración. Puedes especificar variables de entorno, argumentos de línea de comandos y más.
```
pm2 start app.js --name="mi-aplicacion" -- --puerto 3000
```

PM2 se integra fácilmente con otros componentes del ecosistema Node.js, como Keymetrics para la monitorización avanzada y PM2 Plus para funciones adicionales.
