# 🐞 Bugs – Campo `ID` en el cuerpo JSON

📌 **Nota:** Este es un ejercicio de práctica. Los Bug IDs son simulados y no contienen enlaces reales a Jira.

---

### Caso 8 – Campo `ID` acepta letras

**Endpoint:** `POST /api/v1/kits/{id}/products`  

**Datos enviados:**
```json
{
  "id": "abc"
}
Esperado:

Código: 400 Bad Request

Error de validación por tipo de dato

Obtenido:

Código: 200 OK

Sin error, listado mostrado

Estado: ❌ FAILED
Bug ID: ENP2-6 (ficticio)

Caso 9 – Campo ID acepta número decimal
Endpoint: POST /api/v1/kits/{id}/products

Datos enviados:

json
Copy code
{
  "id": 45.9
}
Esperado:

Código: 400 Bad Request

Mensaje de error

Obtenido:

Código: 200 OK

Sin error, listado mostrado

Estado: ❌ FAILED
Bug ID: ENP2-13 (ficticio)

Caso 10 – Campo ID acepta número negativo
Endpoint: POST /api/v1/kits/{id}/products

Datos enviados:

json
Copy code
{
  "id": -12
}
Esperado:

Código: 400 Bad Request

Mensaje de error

Obtenido:

Código: 200 OK

Sin error, listado mostrado

Estado: ❌ FAILED
Bug ID: ENP2-13 (ficticio)

Caso 48 – Campo ID con longitud 3 no muestra listado
Endpoint: PUT /api/v1/orders/:id

Datos enviados:

json
Copy code
{
  "id": 123
}
Esperado:

Código: 200 OK con listado mostrado

Obtenido:

Código: 200 OK pero sin listado

Estado: ❌ FAILED
Bug ID: ENP2-1 (ficticio)

yaml
Copy code

---

### 📁 Carpeta: `/productsWeight/README.md`

```md
# 🐞 Bug – Campo `productsWeight` acepta letras

📌 **Nota:** Este es un ejercicio de práctica. El Bug ID es simulado y no contiene un enlace real a Jira.

**ID del caso:** 33  
**Endpoint:** `POST /order-and-go/v1/delivery`  

## Descripción  
El campo `productsWeight` debe aceptar solo valores numéricos. Se ingresaron letras y la petición fue aceptada.

## Datos enviados
```json
{
  "productsWeight": "abc"
}
Resultado esperado
Código 400 Bad Request

Mensaje de error

No se genera listado

Resultado obtenido
Código 200 OK

Sin mensaje de error

Se genera listado incorrectamente

Estado: ❌ FAILED
Bug ID: ENP2-14 (ficticio)

yaml
Copy code

---

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
📁 Carpeta: /productsCount/README.md
md
Copy code
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
📁 Carpeta: /id_en_url/README.md
md
Copy code
# 🐞 Bugs – Validación del campo ID en la URL

📌 **Nota:** Este es un ejercicio de práctica. Los Bug IDs son simulados y no contienen enlaces reales a Jira.

---

### Caso 35 – ID no existente devuelve 200 OK

**Endpoint:** `GET /api/v1/orders/:id`  

**Esperado:**  
- Código `404 Not Found`  

**Obtenido:**  
- Código `200 OK`  

**Estado:** ❌ FAILED  
**Bug ID:** ENP2-20 *(ficticio)*

---

### Caso 37 – Token no autorizado permite acceso

**Endpoint:** `GET /api/v1/orders/:id`

**Esperado:**  
- Código `401 Unauthorized`  

**Obtenido:**  
- Código `200 OK`  

**Estado:** ❌ FAILED  
**Bug ID:** ENP2-21 *(ficticio)*

---

### Caso 40 – PUT no muestra listado

**Endpoint:** `PUT /api/v1/orders/:id`

**Esperado:**  
- Código `200 OK` con listado  

**Obtenido:**  
- Código `200 OK` sin listado  

**Estado:** ❌ FAILED  
**Bug ID:** ENP2-22 *(ficticio)*

---

### Caso 43 – ID con letras es aceptado

**Endpoint:** `PUT /api/v1/orders/:id`

**Esperado:**  
- Código `400 Bad Request`  

**Obtenido:**  
- Código `200 OK`  

**Estado:** ❌ FAILED  
**Bug ID:** ENP2-25 *(ficticio)*

---

Caso 9 – Campo ID acepta número decimal
Endpoint: POST /api/v1/kits/{id}/products

Datos enviados:

json
Copy code
{
  "id": 45.9
}
Esperado:

Código: 400 Bad Request

Mensaje de error

Obtenido:

Código: 200 OK

Sin error, listado mostrado

Estado: ❌ FAILED
Bug ID: ENP2-13 (ficticio)

Caso 10 – Campo ID acepta número negativo
Endpoint: POST /api/v1/kits/{id}/products

Datos enviados:

json
Copy code
{
  "id": -12
}
Esperado:

Código: 400 Bad Request

Mensaje de error

Obtenido:

Código: 200 OK

Sin error, listado mostrado

Estado: ❌ FAILED
Bug ID: ENP2-13 (ficticio)






