# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 21 correctas de 26 queries

## ❌ Query 1: Incorrecto
```diff
--- 
+++ 
@@ -1,12 +1,12 @@
-nombre
-Disco duro SATA3 1TB
-Memoria RAM DDR4 8GB
-Disco SSD 1 TB
-GeForce GTX 1050Ti
-GeForce GTX 1080 Xtreme
-Monitor 24 LED Full HD
-Monitor 27 LED Full HD
-Portátil Yoga 520
-Portátil Ideapd 320
-Impresora HP Deskjet 3720
-Impresora HP Laserjet Pro M26nw
+codigo | nombre | precio | codigo_fabricante
+1.00 | Disco duro SATA3 1TB | 86.99 | 5.00
+2.00 | Memoria RAM DDR4 8GB | 120.00 | 6.00
+3.00 | Disco SSD 1 TB | 150.99 | 4.00
+4.00 | GeForce GTX 1050Ti | 185.00 | 7.00
+5.00 | GeForce GTX 1080 Xtreme | 755.00 | 6.00
+6.00 | Monitor 24 LED Full HD | 202.00 | 1.00
+7.00 | Monitor 27 LED Full HD | 245.99 | 1.00
+8.00 | Portátil Yoga 520 | 559.00 | 2.00
+9.00 | Portátil Ideapd 320 | 444.00 | 2.00
+10.00 | Impresora HP Deskjet 3720 | 59.99 | 3.00
+11.00 | Impresora HP Laserjet Pro M26nw | 180.00 | 3.00
```

⏱ Tiempo: 0.34 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 3: Incorrecto
```diff
--- 
+++ 
@@ -1,12 +1,5 @@
-codigo | nombre | precio | codigo_fabricante
-1.00 | Disco duro SATA3 1TB | 86.99 | 5.00
-2.00 | Memoria RAM DDR4 8GB | 120.00 | 6.00
-3.00 | Disco SSD 1 TB | 150.99 | 4.00
-4.00 | GeForce GTX 1050Ti | 185.00 | 7.00
-5.00 | GeForce GTX 1080 Xtreme | 755.00 | 6.00
-6.00 | Monitor 24 LED Full HD | 202.00 | 1.00
-7.00 | Monitor 27 LED Full HD | 245.99 | 1.00
-8.00 | Portátil Yoga 520 | 559.00 | 2.00
-9.00 | Portátil Ideapd 320 | 444.00 | 2.00
-10.00 | Impresora HP Deskjet 3720 | 59.99 | 3.00
-11.00 | Impresora HP Laserjet Pro M26nw | 180.00 | 3.00
+Field | Type | Null | Key | Default | Extra
+codigo | int unsigned | NO | PRI | NULL | auto_increment
+nombre | varchar(100) | NO |  | NULL | 
+precio | double | NO |  | NULL | 
+codigo_fabricante | int unsigned | NO | MUL | NULL | 
```

## ❌ Query 3: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'SHOW COLUMNS FROM producto' at line 2


## ✅ Query 4: Correcto

⏱ Tiempo: 0.28 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 5: Correcto

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 6: Correcto

⏱ Tiempo: 0.28 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 7: Correcto

⏱ Tiempo: 0.27 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 8: Correcto

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 9: Correcto

⏱ Tiempo: 0.28 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 10: Correcto

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 11: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 12: Correcto

⏱ Tiempo: 0.28 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

---

## ✅ Query 13: Correcto

⏱ Tiempo: 0.28 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 14: Correcto

⏱ Tiempo: 0.28 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 15: Correcto

⏱ Tiempo: 0.28 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 16: Correcto

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ✅ Query 17: Correcto

⏱ Tiempo: 0.27 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ✅ Query 18: Correcto

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 19: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 20: Correcto

⏱ Tiempo: 0.29 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

---

## ✅ Query 21: Correcto

⏱ Tiempo: 0.31 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 22: Incorrecto
```diff
--- 
+++ 
@@ -1,12 +1,12 @@
 nombre | precio | nombre del fabricante
+Disco duro SATA3 1TB | 86.99 | Seagate
+Disco SSD 1 TB | 150.99 | Samsung
+GeForce GTX 1050Ti | 185.00 | Gigabyte
+GeForce GTX 1080 Xtreme | 755.00 | Crucial
+Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
+Impresora HP Laserjet Pro M26nw | 180.00 | Hewlett-Packard
+Memoria RAM DDR4 8GB | 120.00 | Crucial
 Monitor 24 LED Full HD | 202.00 | Asus
 Monitor 27 LED Full HD | 245.99 | Asus
-Memoria RAM DDR4 8GB | 120.00 | Crucial
-GeForce GTX 1080 Xtreme | 755.00 | Crucial
-GeForce GTX 1050Ti | 185.00 | Gigabyte
-Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
-Impresora HP Laserjet Pro M26nw | 180.00 | Hewlett-Packard
+Portátil Ideapd 320 | 444.00 | Lenovo
 Portátil Yoga 520 | 559.00 | Lenovo
-Portátil Ideapd 320 | 444.00 | Lenovo
-Disco SSD 1 TB | 150.99 | Samsung
-Disco duro SATA3 1TB | 86.99 | Seagate
```

⏱ Tiempo: 0.32 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ✅ Query 23: Correcto

⏱ Tiempo: 0.30 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 24: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,2 @@
-nombre | precio | fabricant
+nombre | precio | fabricante
 Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
```

⏱ Tiempo: 0.31 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ✅ Query 25: Correcto

⏱ Tiempo: 0.30 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 26: Error
- **Descripción**: 'NoneType' object is not iterable

