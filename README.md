# 🛰️ Plataforma Sentinel

[![Documento en vivo](https://img.shields.io/badge/leer-geovanilozano.github.io%2Fsentinel-1f6feb?style=flat-square&logo=github)](https://geovanilozano.github.io/sentinel/)
[![GitHub Pages](https://img.shields.io/badge/deploy-GitHub%20Pages-222?style=flat-square&logo=githubpages)](https://geovanilozano.github.io/sentinel/)
[![Material propietario](https://img.shields.io/badge/licencia-propietaria-b45309?style=flat-square)](#-licencia)

> Documento técnico de **Sentinel**, la plataforma de gestión y diagnóstico de
> activos solares de SAMS Technology: arquitectura, gobierno de datos, modelo de
> KPIs y el motor matemático que sostiene el diagnóstico energético.

## 📖 Leer el documento

**[geovanilozano.github.io/sentinel](https://geovanilozano.github.io/sentinel/)**

Es una sola página autocontenida: sin dependencias, sin build y sin JavaScript de
terceros. Se abre igual desde el navegador que desde un `file://` local, lo que
permite enviarla a un cliente sin pedirle que instale nada.

## 🗂️ Qué contiene

| Sección | De qué trata |
|---|---|
| **La plataforma en una página** | Resumen ejecutivo y alcance |
| **Módulos de la plataforma** | Descomposición funcional del sistema |
| **La cadena del dato** | Del inversor al KPI: ingesta, normalización y consumo |
| **Gobierno y calidad del dato** | Propiedad, trazabilidad y reglas de validación |
| **Modelo de datos del diagnóstico** | Entidades y relaciones del dominio |
| **El motor matemático** | Disponibilidad, pérdidas, modelo físico y causa raíz |
| **Catálogo de ecuaciones** | Las fórmulas, con sus supuestos explícitos |
| **Ejecución y entregables** | Cómo corre y qué produce |
| **Integraciones y entornos** | Interfaces externas y despliegue |
| **Estado real de la implementación** | Qué está construido y qué no |

La última sección es deliberada: el documento distingue lo diseñado de lo
efectivamente construido, para que sirva como referencia honesta y no como folleto.

## 🏗️ Estructura del repositorio

```
index.html    Documento completo (HTML + CSS embebidos)
robots.txt    Reglas de indexación
.nojekyll     Publica el HTML tal cual, sin procesar con Jekyll
```

## 🚀 Despliegue

GitHub Pages sirve la rama `main` desde la raíz. Cada `push` republica el sitio;
no hay paso de compilación.

```bash
git clone https://github.com/geovanilozano/sentinel.git
cd sentinel
# Abrir index.html en el navegador, o servirlo:
python -m http.server 8000
```

## 🔗 Proyectos relacionados

- **[sams-2.0](https://github.com/geovanilozano/sams-2.0)** — implementación de la plataforma (Turborepo + NestJS + Next.js + TimescaleDB)
- **[SAMS-ENERGY-DIAGNOSTIC-ENGINE](https://github.com/geovanilozano/SAMS-ENERGY-DIAGNOSTIC-ENGINE)** — microservicio del motor matemático (Python + PVLib)

## 📄 Licencia

**Material propietario de SAMS Technology. Todos los derechos reservados.**

Este documento describe la arquitectura, el gobierno de datos y el motor de
cálculo de una plataforma comercial, y está elaborado a partir de sus
repositorios privados. No se concede licencia de uso, copia, modificación ni
redistribución.

---

<p align="center">
  <sub>Escrito por <a href="https://github.com/geovanilozano">Geovani Lozano</a> · CTO, SAMS Technology</sub>
</p>
