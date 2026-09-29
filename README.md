# EcoGrow
Plataforma web para la gestión, geolocalización de huertos

## Riesgos del Proyecto 

| ID | Riesgo | Probabilidad | Impacto | Nivel | Plan de Mitigación | Plan de Contingencia |
| :--- | :--- | :---: | :---: | :---: | :--- | :--- |
| **R1** | Falla de internet en zonas de huertos | Alta | Alto | **Crítico** | Diseñar como PWA para guardar datos e itinerarios de forma local. | Sincronizar los datos automáticamente cuando el dispositivo recupere señal. |
| **R2** | Falla o imprecisión en la ubicación GPS | Media | Alto | **Alto** | Permitir ajustar el pin del huerto manualmente sobre el mapa. | Incluir referencias en texto y enlace a Google Maps / Waze. |
| **R3** | Caída del servicio de mapas | Baja | Alto | **Medio** | Usar bibliotecas *open-source* (Leaflet) con servidores de respaldo. | Cambiar el proveedor de mapas en el frontend sin cerrar la sesión. |
| **R4** | Demoras en la API de rutas (OSRM) | Media | Medio | **Medio** | Poner tiempos límite de espera (*timeouts*) en las peticiones. | Ordenar paradas por distancia directa (Haversine) si falla la API. |
| **R5** | Dificultad de uso para dueños de huertos | Media | Alto | **Alto** | Diseñar una pantalla simple con botones grandes y pasos claros. | Permitir que un administrador apoye registrando el inventario. |
| **R6** | Cancelaciones de recolección a última hora | Alta | Medio | **Alto** | Enviar alertas y pedir confirmación obligatoria previa. | Reabrir la oferta a otros recolectores cercanos si la reserva expira. |
