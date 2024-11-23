---
title: "Contenidos"
date: 2024-11-17
draft: false

---

# Introducción al Lenguaje PHP 🐘

PHP (acrónimo de *Hypertext Preprocessor*) es un lenguaje de programación de propósito general diseñado para el desarrollo web. Se ejecuta en el servidor y se utiliza para generar contenido dinámico en páginas web.

---

## 1. ¿Qué es PHP? 🤔

PHP es un lenguaje de programación:
- **Interpretado**: No requiere compilación.
- **Orientado al servidor**: Se ejecuta en el servidor y genera HTML para el cliente.
- **Ampliamente usado**: Popular en la creación de sitios web dinámicos.

### **Ventajas de PHP**
- Fácil de aprender.
- Amplia compatibilidad con servidores y bases de datos.
- Gran comunidad y recursos de soporte.
- Integración sencilla con HTML y CSS.

### **Primer programa en PHP**
El código básico en PHP se escribe dentro de etiquetas `<?php ... ?>`.

```php
<?php
echo "¡Hola, mundo!";
// Esto mostrará "¡Hola, mundo!" en el navegador
```
## 2. Sintaxis Básica 📝

### **Variables**

```php
<?php
$nombre = "Juan";
$edad = 30;
echo "Me llamo $nombre y tengo $edad años.";
?>
```

### **Tipos de Datos**

String: Cadenas de texto.<br>

Int: Números enteros.

Float: Números decimales.

Bool: Booleanos (true/false).

Array: Listas de elementos.

Object: Objetos.

```php
<?php
$cadena = "Texto";
$numero = 42;
$decimal = 3.14;
$booleano = true;
$array = [1, 2, 3, 4];
?>
```