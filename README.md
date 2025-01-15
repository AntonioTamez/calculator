# Calculadora Vue.js

## Descripción
Esta aplicación es una **calculadora moderna** desarrollada con Vue.js que incluye las funcionalidades esenciales para realizar cálculos matemáticos. Además, presenta un diseño responsivo, intuitivo y profesional, compatible con dispositivos móviles, tabletas y computadoras de escritorio.

---

## Demo

---

## Características principales

- **Operaciones básicas**:
  - Suma, resta, multiplicación, división.
  - Cálculo de porcentajes.
- **Historial de operaciones**:
  - Guarda todas las operaciones realizadas junto con sus resultados.
  - Incluye la opción de limpiar el historial.
- **Evaluación de expresiones completas**:
  - Permite ingresar y resolver expresiones como `60 + 25%`.
- **Diseño moderno y responsivo**:
  - Adaptable a cualquier tamaño de pantalla.
  - Uso de colores atractivos y una interfaz clara.
- **Opciones de reinicio**:
  - Limpieza de la operación actual o reinicio completo del estado de la calculadora.

---

## Tecnologías utilizadas

- **Framework**: Vue.js (última versión disponible).
- **Estilos**: CSS moderno con diseño responsivo.
- **Gestión del estado**: Composition API (para manejar el estado de la aplicación y el historial).

---

## Instalación y configuración

### Prerrequisitos

- **Node.js** (versión 14 o superior).
- **npm** (versión 7 o superior) o **Yarn**.

### Pasos para instalar y ejecutar

1. **Clona este repositorio**:
   ```bash
   git clone https://github.com/AntonioTamez/calculator.git
   cd calculator
   ```

2. **Instala las dependencias**:
   ```bash
   npm install
   # o con Yarn
   yarn install
   ```

3. **Ejecuta el servidor de desarrollo**:
   ```bash
   npm run dev
   # o con Yarn
   yarn dev
   ```

4. **Abre la aplicación en tu navegador**:
   - Ve a `http://localhost:5173`.

---

## Uso

1. Ingresa números y selecciona las operaciones deseadas usando los botones.
2. Utiliza `%` para calcular porcentajes.
   - Ejemplo: `60 * 25%` mostrará el resultado `15`.
3. Presiona `=` para obtener el resultado de la operación.
4. Consulta el historial para revisar operaciones previas.
5. Usa `C` para borrar la entrada actual o `AC` para reiniciar completamente la calculadora.

---

## Estructura del proyecto

- `App.vue`: Componente principal que contiene la lógica y diseño de la calculadora.
- `main.js`: Archivo de entrada para inicializar la aplicación Vue.
- `assets/styles.css`: Archivo de estilos para personalizar el diseño.

---

## Contribución

¡Contribuciones son bienvenidas! Sigue estos pasos:

1. Haz un **fork** del repositorio.
2. Crea una **rama nueva** con tus cambios:
   ```bash
   git checkout -b mi-nueva-funcionalidad
   ```
3. Guarda tus cambios y súbelos al repositorio remoto:
   ```bash
   git push origin mi-nueva-funcionalidad
   ```
4. Abre un **pull request**.

---

## Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.
