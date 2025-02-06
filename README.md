# Juego Adivinanzas Árbol de Nodos

Este es un juego de adivinanzas basado en un árbol de decisión, donde el programa intentará adivinar un personaje a través de preguntas. Si no lo adivina, el usuario puede enseñar nuevas preguntas y respuestas al sistema, permitiendo que aprenda con el tiempo.

## Estructura del Proyecto

```
Juego-Adivinanzas-Arbol-Nodos/
│── backup.txt
│── conocimiento.txt
│── conocimientofallido.txt // Este borrenlo
│── pom.xml
│── src/main/java/programaListo/
│   ├── ArbolNodos.java
│   ├── Archivo.java
│   ├── Main.java
│   ├── Nodo.java
```

### Archivos principales

- **ArbolNodos.java**: Implementación de un árbol binario de decisión que gestiona las preguntas y respuestas.
- **Archivo.java**: Manejo de la serialización y deserialización del árbol en un archivo para persistencia de datos.
- **Main.java**: Lógica del juego, interacción con el usuario y aprendizaje del sistema.
- **Nodo.java**: Representa los nodos del árbol, los cuales pueden ser preguntas o respuestas.
- **backup.txt**: Archivo de respaldo de los datos del sistema.
- **conocimiento.txt**: Archivo donde se guarda el conocimiento aprendido.
- **pom.xml**: Archivo de configuración para Maven.

## Requisitos

- Java 8 o superior
- Maven (opcional, si se usa para gestionar dependencias)

## Ejecución

1. Compila los archivos Java:
   ```sh
   javac -d bin src/main/java/programaListo/*.java
   ```
2. Ejecuta el programa:
   ```sh
   java -cp bin programaListo.Main
   ```

Si usas Maven, puedes ejecutar:
   ```sh
   mvn compile exec:java -Dexec.mainClass="programaListo.Main"
   ```

## Funcionamiento del Juego

1. El programa comienza con una pregunta base.
2. Si el programa adivina correctamente el personaje, gana.
3. Si no, el usuario puede introducir una nueva pregunta y respuesta para mejorar el sistema.
4. Los datos se guardan en `conocimiento.txt` para ser utilizados en futuras ejecuciones.

## Contribución

Si deseas contribuir, puedes hacer un fork del repositorio y enviar un pull request con mejoras en el código o en la lógica del juego.

## Autor

Desarrollado por **Junior**.

