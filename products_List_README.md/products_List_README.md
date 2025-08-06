### 📁 Carpeta: `/productsList/README.md`

```md
# 🐞 Bug – Campo `productsList` vacío es aceptado

📌 **Nota:** Este es un ejercicio de práctica. El Bug ID es simulado y no contiene un enlace real a Jira.

**ID del caso:** 17  
**Endpoint:** `POST /api/v1/kits/{id}/products`

## Descripción  
El campo `productsList` fue enviado vacío o mal formado y no se validó.

## Resultado esperado
- Código `400 Bad Request`  
- Mensaje de error

## Resultado obtenido
- Código `200 OK`  
- Sin mensaje de error  

**Estado:** ❌ FAILED  
**Bug ID:** ENP2-31 *(ficticio)*
