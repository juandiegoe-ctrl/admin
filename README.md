# ADMIN ESTONA · Consolidado

El portal ahora usa la misma estructura de la hoja `Consolidado`:

- Tipo de documento
- Fecha Emisión
- NIT Emisor
- Nombre Emisor
- Descripción
- IVA
- Total
- Categoría

Se prepararon 1142 registros históricos del Consolidado.

## Instalación

1. Ejecuta `02_consolidado_egresos.sql` en Supabase.
2. Reemplaza `index.html` de ADMIN ESTONA.
3. Recarga `admin.estona.co`.

El SQL es idempotente: si lo ejecutas dos veces, `source_key` evita duplicar el histórico.

## Dashboard

Muestra:
- Egresos del mes
- IVA del mes
- Documentos
- Emisores
- Gastos por categoría
- Principales egresos

Las categorías se normalizaron quitando espacios sobrantes.
