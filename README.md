# EcoGrow
Plataforma web para la gestión, geolocalización de huertos

## Riesgos 

| ID | Riesgo | Probabilidad | Impacto | Nivel | ¿Cómo prevenirlo?  | ¿Qué se hace si llega a pasar??  |
| :--- | :--- | :---: | :---: | :---: | :--- | :--- |
| **R1** | **Falta de señal / internet en los huertos** | Alta | Alto | **Crítico** | Hacer que la página guarde datos básicos en la memoria del navegador para que no se trabe sin señal. | Dejar que el usuario guarde su información y hacer que se envíe sola cuando vuelva a tener internet. |
| **R2** | **Que el GPS no dé la ubicación exacta del huerto** | Media | Alto | **Alto** | Dejar que el usuario mueva manualmente el pin en el mapa para marcar el punto exacto. | Mostrar la dirección escrita en texto y poner un botón para abrir el mapa directo en Google Maps o Waze. |
| **R3** | **Que el servicio de mapas se caiga o falle** | Baja | Alto | **Medio** | Usar librerías libres (como Leaflet) que permiten conectar varios proveedores de mapas de respaldo. | Si un mapa falla, cambiar automáticamente a otro servidor sin cerrar la sesión del usuario. |
| **R4** | **Que el cálculo de la ruta de recolección tarde mucho** | Media | Medio | **Medio** | Poner un límite de tiempo de espera a la consulta de rutas para que la página no se quede congelada. | Si falla el cálculo de rutas, ordenar los huertos por cercanía en línea recta para no dejar al usuario sin respuesta. |
| **R5** | **Que a los dueños de los huertos se les complique usar la página** | Media | Alto | **Alto** | Diseñar pantallas muy sencillas con botones grandes, textos claros y pocos pasos. | Permitir que un administrador o el mismo recolector pueda ayudarles a registrar la cosecha. |
| **R6** | **Que aparten una cosecha y al final no vayan por ella** | Alta | Medio | **Alto** | Enviar alertas y pedir una confirmación obligatoria antes de liberar la recolección. | Si la reserva vence y nadie confirma, liberar la cosecha otra vez en el mapa para que alguien más la aproveche. |
