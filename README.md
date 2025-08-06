
---

## 📁  `Bugs_API_EvelynNava` → `README.md`

```md
# 🐞 Reporte de Bugs en API – Evelyn Nava

Este repositorio contiene la documentación de **bugs encontrados durante pruebas manuales** a una API de gestión de pedidos. Cada error está detallado en formato profesional como si se tratara de un entorno real de desarrollo.

Los errores fueron encontrados como parte de una práctica personal para fortalecer mis habilidades como **QA Tester Manual**.

---

## 📋 Contenido

- Descripción del error
- Datos enviados
- Resultado esperado
- Resultado obtenido
- Estado final
- Bug ID simulado

---

## 📂 Estructura del repositorio

📦 Bugs_API_EvelynNava
├── id_en_url/
├── id_en_json/
├── productsList/
├── productsCount/
├── productsWeight/
├── orders/
├── README.md  ← Este archivo
📌 Importante
Todos los bugs están documentados con IDs simulados (ej. ENP2-03). No corresponden a un Jira real, pero están escritos con estándares profesionales.

🧪 Ejemplo de bug documentado

# 🐞 Bug – El sistema permite ID negativo en la URL

**ID del caso:** 5  
**Endpoint:** `POST /api/v1/kits/{id}/products`  
**Resultado esperado:** Código 400 / Mensaje de error  
**Resultado obtenido:** Código 200 OK / Se muestra listado  
**Estado:** ❌ FAILED  
**Bug ID simulado:** ENP2-03  
👩‍💻 Autora
Evelyn Nava García
Documentación de errores funcionales en APIs
📍 CDMX, México
