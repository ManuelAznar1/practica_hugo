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

String: Cadenas de texto.

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

## 3. Control de Flujo 🚦

### **Condicionales**

Se utiliza if, else y elseif para controlar el flujo del programa.

```php
<?php
$edad = 20;

if ($edad >= 18) {
    echo "Eres mayor de edad.";
} else {
    echo "Eres menor de edad.";
}
?>
```

### **Bucles**

Los bucles permiten ejecutar un bloque de código varias veces.

#### Bucle for
```php
<?php
for ($i = 0; $i < 5; $i++) {
    echo "El número es: $i <br>";
}
?>
```

#### Bucle while
```php
<?php
$i = 0;
while ($i < 5) {
    echo "El número es: $i <br>";
    $i++;
}
?>
```

## 4. Funciones en PHP 🔧

Las funciones encapsulan bloques de código para ser reutilizados.

```php
<?php
function saludo($nombre) {
    return "Hola, $nombre!";
}

echo saludo("Ana");
?>
```

## 5. Manejo de Formularios ✉️

PHP puede procesar datos enviados desde formularios HTML.

#### Formulario HTML

```html
<form action="procesar.php" method="POST">
    <label for="nombre">Nombre:</label>
    <input type="text" id="nombre" name="nombre">
    <button type="submit">Enviar</button>
</form>
```

#### Procesamiento en PHP

```php
<?php
$nombre = $_POST['nombre'];
echo "Hola, $nombre!";
?>
```

## 6. Conexión a Bases de Datos 📊

PHP se integra fácilmente con bases de datos como MySQL.

Ejemplo de conexión a MySQL:

```php
<?php
$host = "localhost";
$usuario = "root";
$contraseña = "";
$base_datos = "mi_base";

$conn = new mysqli($host, $usuario, $contraseña, $base_datos);

if ($conn->connect_error) {
    die("Conexión fallida: " . $conn->connect_error);
}

echo "Conexión exitosa.";
?>
```

## 7. Buenas Prácticas en PHP ✅

#### Uso de comentarios:

```php
    Comentario de una línea: // Esto es un comentario.
    Comentario de múltiples líneas:

    /*
    Este es un comentario
    de varias líneas.
    */
```

#### Validar entradas del usuario:

```php
<?php
$usuario = htmlspecialchars($_POST['usuario']);
?>
```

## 8. Recursos para Aprender PHP 📚

Aquí tienes algunos recursos importantes sobre PHP:

- [PHP.net](https://www.php.net/): Sitio oficial de PHP con documentación y tutoriales.
- [W3Schools PHP](https://www.w3schools.com/php/): Tutoriales interactivos para aprender PHP.
- [Tutorial de PHP en GeeksforGeeks](https://www.geeksforgeeks.org/php/): Guía completa con ejemplos y buenas prácticas.
- [Stack Overflow PHP Questions](https://stackoverflow.com/questions/tagged/php): Preguntas frecuentes y soluciones de la comunidad.
- [PHP: The Right Way](https://phptherightway.com/): Guía recomendada para seguir buenas prácticas en PHP.