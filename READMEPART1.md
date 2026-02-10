# Graceful Offline Mode
## Parte 1 del laboratorio
### Link del video de explicación: 
En esta parte se modifico el proyecto para que el programa guarde datos de la API en el caché si fueron cargados previamente al tener conexión de internet.
Tambien se modifico para que el programa fuera capaz de mostrar los datos guardados en el caché en caso de que no hubiera conexión a internet.
| Criterio                          | Descripción                                                                |
| --------------------------------- | -------------------------------------------------------------------------- |
| Estado de la UI actualizado       | El estado de error acepta el opcional: `List<Amiibo>?`                |
| Datos en caché preservados        | El estado de error conserva los datos existentes del estado anterior       |
| Snackbar mostrado                 | El error de red muestra un Snackbar, no un error de pantalla completa       |
| Cuadrícula aún visible            | El usuario ve los Amiibos en caché mientras el Snackbar está activo        |
| Error completo solo si está vacío | El error a pantalla completa se muestra solo si los datos son nulos/vacíos |
| Reintentar disponible             | El Snackbar tiene un botón de acción "Reintentar"                          |
| Descartar funciona                | El Snackbar puede ser descartado sin afectar la cuadrícula                 |

## Definition of Done
