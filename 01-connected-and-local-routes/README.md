# Laboratorio 01: Rutas Conectadas y Locales (Connected and Local Routes)

## 📌 Descripción General
Laboratorio diseñado en **GNS3** para comprender el funcionamiento y la diferencia entre las **rutas conectadas** (*connected routes*) y las **rutas locales** (*local routes*) en una tabla de enrutamiento de un router (R1).

## 📐 Topología de Red
* **Router (R1):** Dispositivo central que maneja las interfaces conectadas a diferentes segmentos.
* **Interfaces y Redes:**
  * `g1/0`: `10.0.1.1/24` (Conectada a Switch1 y PC1: `10.0.1.10`)
  * `g2/0`: `10.0.2.1/24` (Conectada a Switch2 y PC2: `10.0.2.10`)
  * `f0/0`: `10.0.0.1/24` (Conectada a Switch3)
* **Dispositivos Finales (VPCS):**
  * `PC1`: `10.0.1.10/24`
  * `PC2`: `10.0.2.10/24`

## ⚙️ Verificación y Comandos Clave
Para visualizar cómo el router aprende directamente estas redes, se utilizó el siguiente comando en R1:
```text
show ip route
