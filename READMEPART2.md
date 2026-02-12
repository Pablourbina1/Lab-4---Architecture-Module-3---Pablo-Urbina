# Local Search
## Parte 2 del laboratorio
#### Link del video de explicación: https://drive.google.com/file/d/17-O3NSMk2vSSf3l902ze3AUQ-OP4mKLt/view?usp=drive_link
En esta parte se añadio una barra de busqueda al proyecto, la cual permite filtrar amiibos segun el input del usuario, enseñando los amigos que cumplen con dicho input (ejemplo "Mario"
muestra los amiibos que tienen "Mario" en su nombre), el input no muestra nada si se ingresa algo que no hace match con ningun amiibo, y hay una x que borra todo el contenido de la
barra de busqueda cuando es presionada.

## Definition of Done
| Criterio                | Descripción                                                                  |
| ----------------------- | ---------------------------------------------------------------------------- |
| Método DAO existe    | `searchAmiibos(query: String): Flow<List<AmiiboEntity>>`                     |
| Consulta LIKE funciona  | La consulta SQL usa `WHERE name LIKE '%'`                                    |
| TextField de búsqueda   | `OutlinedTextField` en la parte superior de la pantalla                      |
| Filtrado en tiempo real | Los resultados se actualizan mientras el usuario escribe (debounce opcional) |
| Cambio de Flow          | Usa `flatMapLatest` para cambiar entre flujos                                |
| Consulta vacía = todos  | Búsqueda en blanco muestra la lista completa                             |
| Botón limpiar           | Ícono "X" para limpiar el texto de búsqueda                                  |
