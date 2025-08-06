# 🐞 Bug: Campo `productsWeight` acepta letras

**ID del caso:** 33  
**Endpoint:** `POST /order-and-go/v1/delivery`  

## ❓ Descripción
El campo `productsWeight` acepta letras latinas como valor, lo cual no es válido.

### 🔢 Datos usados
```json
{
  "productsWeight": "abc"
✅ Resultado esperado
Código de respuesta: 400 Bad Request

No se debe aceptar el valor ingresado

Se debe mostrar un mensaje de error

No se debe generar un listado

❌ Resultado obtenido
Código de respuesta: 200 OK

La respuesta no muestra errores

Se muestra listado como si la solicitud fuera válida

🧾 Estado final: FAILED
Bug ID simulado: ENP2-14 (referencia ficticia para seguimiento de errores)