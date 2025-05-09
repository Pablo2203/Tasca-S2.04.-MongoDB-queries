# 📘 Ejercicios de Consultas MongoDB: Restaurantes en Nueva York

Este repositorio contiene ejercicios prácticos para realizar consultas en MongoDB sobre una colección que almacena información de restaurantes en la ciudad de Nueva York. El objetivo es desarrollar habilidades en la creación de consultas eficientes y correctas sobre bases de datos NoSQL.

---

## 📄 Descripción - Enunciado del Ejercicio

Se proporciona una colección de datos en MongoDB que contiene información sobre restaurantes en Nueva York. Se deben escribir consultas para responder a los siguientes casos de uso:

### Casos de Uso:
1. Mostrar todos los documentos en la colección Restaurantes.
2. Mostrar `restaurant_id`, `name`, `borough` y `cuisine` para todos los documentos en la colección Restaurantes.
3. Mostrar `restaurant_id`, `name`, `borough` y `cuisine`, excluyendo el campo `_id` para todos los documentos.
4. Mostrar `restaurant_id`, `name`, `borough` y `zipcode`, excluyendo el campo `_id`.
5. Mostrar todos los restaurantes que están en el Bronx.
6. Mostrar los primeros 5 restaurantes que están en el Bronx.
7. Mostrar los próximos 5 restaurantes después de saltar los primeros 5 del Bronx.
8. Encontrar restaurantes que tienen un resultado superior a 90.
9. Encontrar restaurantes con un resultado mayor a 80 pero menor que 100.
10. Encontrar restaurantes que se encuentran en latitudes menores a -95.754168.
11. Encontrar restaurantes que no preparan comida 'American', tienen puntuación superior a 70 y longitud menor a -65.754168.
12. Realizar este mismo caso **sin utilizar el operador `$and`**.
13. Encontrar restaurantes que no preparan comida 'American', tienen un marcador "A", y no pertenecen a Brooklyn. Mostrar según cuisine en orden descendente.
14. Buscar restaurantes por aquellas palabras que contienen o empiezan/terminan con ciertos caracteres específicos (e.g., "Wil", "ces", "Reg", etc.).
15. Realizar combinaciones de búsquedas avanzadas por borough, cuisine y puntuaciones específicas.
16. Consultar por fechas, coordenadas y propiedades específicas relacionadas con el formato de los documentos, grades y más.
17. Organizar los resultados en orden ascendente/descendente por diferentes campos.
18. Seleccionar documentos por tipos de datos específicos y realizar consultas avanzadas relacionadas al uso de expresiones regulares (`$regex`) y operadores matemáticos.

Se agrupa el desarrollo de las consultas en **tres niveles de dificultad**:
- **Nivel 1**: 17 consultas correctas.
- **Nivel 2**: Entre 17 y 25 consultas correctas.
- **Nivel 3**: Más de 25 consultas correctas.

---

## 💻 Tecnologías Utilizadas

- **MongoDB**: Motor de base de datos NoSQL utilizado en el desarrollo de las consultas.
- **MongoDB Compass**: Interfaz gráfica para realizar las consultas directamente sobre la base de datos.
- **Shell de MongoDB (CLI)**: Para ejecutar y probar las consultas en un entorno de línea de comandos.
- **JavaScript**: Sintaxis de consultas dentro del entorno de MongoDB.

---

## 📋 Requisitos

Antes de comenzar, asegúrate de cumplir con los siguientes requisitos:

1. Tener correctamente instalado **MongoDB**. Puedes descargarlo [aquí](https://www.mongodb.com/try/download/community).
2. Tener acceso a **MongoDB Compass** o cualquier cliente para conectarte y realizar consultas fácilmente.
3. Cargar la base de datos de ejemplo proporcionada en el archivo adjunto:
   - Descarga el archivo `restaurants.json` (o el archivo que contiene los datos).
   - Usa el siguiente comando para importar la colección (suponiendo que tengas la CLI instalada):
     ```bash
     mongoimport --db nombre_base_datos --collection nombre_coleccion --file ruta_al_archivo.json
     ```

---

## 🛠️ Instalación

1. Clona este repositorio en tu máquina local:
   ```bash
   git clone https://github.com/tu-usuario/tu-repositorio.git
   cd tu-repositorio
   ```

2. Carga los datos en MongoDB, como se indica en los requisitos.

3. Abre **MongoDB Compass** o la shell de MongoDB para conectarte a tu instancia de MongoDB.

4. Prueba las consultas una a una dentro del entorno interactivo. Todas las consultas están organizadas en el archivo `queries.js`.

---

## ▶️ Ejecución

1. Asegúrate de que tu servidor MongoDB esté en ejecución (por ejemplo, en el puerto 27017).
2. Usa **MongoDB Compass** o la CLI para conectarte.
3. Ejecuta consultas directamente en MongoDB shell o Compass. Por ejemplo:
   ```js
   db.restaurants.find({})
   ```
4. Las consultas completas están documentadas y organizadas en este repositorio.

---

## 🌐 Despliegue

Este proyecto no requiere despliegue formal. Contiene únicamente consultas orientadas al aprendizaje y modelado de bases de datos con MongoDB. Puedes adaptarlo e implementarlo como parte de un proyecto más grande si fuera necesario.

---

## 🤝 Contribuciones

¡Las contribuciones son bienvenidas! Si detectas errores en las consultas, tienes nuevas ideas o quieres agregar funciones avanzadas, sigue estos pasos:

1. Realiza un **fork** del repositorio.
2. Crea una nueva rama con tus cambios:
   ```bash
   git checkout -b nueva-feature
   ```
3. Realiza el commit con tus cambios:
   ```bash
   git commit -m "Descripción de los cambios realizados"
   ```
4. Envía un **pull request** con una descripción detallada de tus cambios.

---

Si tienes ideas, dudas, comentarios o preguntas, no dudes en abrir un **issue** en este repositorio.

### ¡Gracias por participar y aprender con este ejercicio practico de MongoDB! 🚀
