# 🐞 Bug – Campo `productsCount` vacío es aceptado

📌 **Nota:** Este es un ejercicio de práctica. El Bug ID es simulado y no contiene un enlace real a Jira.

**ID del caso:** 29  
**Endpoint:** `POST /order-and-go/v1/delivery`

## Descripción  
El campo `productsCount` fue enviado sin valor y no se validó.

## Resultado esperado
- Código `400 Bad Request`  
- Mensaje de error

## Resultado obtenido
- Código `200 OK`  
- Sin validación ni error

**Estado:** ❌ FAILED  
**Bug ID:** ENP2-31 *(ficticio)*
