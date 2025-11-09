# 📦 SAT Catalog JSON

Repositorio público con el **catálogo oficial del SAT (Servicio de Administración Tributaria de México)** convertido a formato **JSON**, listo para ser usado en cualquier lenguaje o framework.

Ideal para desarrolladores que trabajan con **CFDI**, **facturación electrónica**, validación de **productos/servicios**, **regímenes fiscales**, **impuestos**, entre otros.

---

## 🚀 Descripción

Este archivo contiene los **catálogos oficiales del SAT** en formato estructurado **JSON**, permitiendo integrarlos fácilmente en sistemas de facturación, validadores o APIs.

Los datos provienen de las fuentes públicas del SAT y se distribuyen con fines educativos y de desarrollo.

---

## 📁 Archivo disponible

| Archivo | Descripción |
|----------|--------------|
| `sat_catalog.json` | Catálogo completo del SAT en formato JSON. |

---

## 🧱 Ejemplo de uso

### Node.js
```ts
import fs from "fs";

const catalog = JSON.parse(fs.readFileSync("./sat_catalog.json", "utf-8"));

// Buscar un régimen fiscal
const regimen = catalog.regimenes.find(r => r.clave === "601");
console.log(regimen.descripcion); // "General de Ley Personas Morales"
