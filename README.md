💱 Conversor de Monedas
Aplicación Android desarrollada en Kotlin con Android Studio, que permite convertir valores entre distintas monedas de manera sencilla y visual. Incluye un diseño moderno con Material Design, botones de intercambio y limpieza, y un splash screen con logo personalizado.
📱 Características principales
✅ Conversión entre 6 monedas (EUR, USD, MXN, ARS, CLP, COP).
✅ Validación de errores (monto vacío, formato incorrecto, mismas monedas).
✅ Botón Intercambiar para cambiar moneda origen ↔ destino.
✅ Botón Limpiar para reiniciar los campos.
✅ Interfaz con Material Design y colores suaves.
✅ Logo personalizado y pantalla de inicio (Splash).
✅ Compatible con pantallas pequeñas y grandes (ConstraintLayout).
🧰 Tecnologías utilizadas
Tipo
Detalle
🧠 Lenguaje
Kotlin
🏗️ IDE
Android Studio
🧩 Layout
ConstraintLayout
🎨 Diseño
Material Design 3
📦 Librerías
androidx.appcompat, com.google.android.material, androidx.core:core-splashscreen
📱 SDK
Compile SDK 34
💾 Compatibilidad mínima
Android 7.0 (API 24)

📂 Estructura del proyecto
📦 ConversorMonedas
 ┣ 📂 app/src/main/java/com/example/conversormonedas/
 ┃ ┗ 📜 MainActivity.kt
 ┣ 📂 app/src/main/res/layout/
 ┃ ┗ 📜 activity_main.xml
 ┣ 📂 app/src/main/res/values/
 ┃ ┣ 📜 arrays.xml
 ┃ ┣ 📜 colors.xml
 ┃ ┗ 📜 themes.xml
 ┣ 📂 app/src/main/res/drawable/
 ┃ ┣ 🎨 ic_logo_app.xml / .png
 ┃ ┣ 🔁 ic_swap_horiz_24.xml
 ┃ ┗ ❌ ic_clear_24.xml
 ┗ 📜 README.md
⚙️ Funcionamiento
1️⃣ Introducir un monto.
2️⃣ Seleccionar moneda origen y destino.
3️⃣ Pulsar Convertir → muestra el resultado con dos decimales.
4️⃣ Intercambiar ↔ invierte las monedas seleccionadas.
5️⃣ Limpiar borra monto y resultado.


El cálculo usa una tasa fija (referenciada al Euro) para simular el comportamiento de un conversor real.
val tasaPorEUR = mapOf(
    "EUR" to 1.0,
    "USD" to 1.08,
    "MXN" to 18.5,
    "ARS" to 955.0,
    "CLP" to 980.0,
    "COP" to 4400.0
)
🎨 Diseño y apariencia
• Fondo con color suave (#FFE3F2FD).
• Logo centrado debajo del título principal.
• Botón principal elevado (MaterialButton).
• Íconos vectoriales (swap_horiz y clear).
• Tema Material 3 con splash screen inicial.
🚀 Instalación y ejecución
1. Clonar el repositorio: git clone https://github.com/tuusuario/ConversorMonedas.git
2. Abrir el proyecto en Android Studio.
3. Sincronizar Gradle.
4. Ejecutar en un emulador o dispositivo físico (Android 7.0+).
🌟 Mejoras futuras
• Obtener tasas de cambio en tiempo real desde una API externa.
• Añadir modo oscuro.
• Guardar histórico de conversiones.
• Agregar traducciones a otros idiomas.
• Permitir compartir el resultado.
🧑‍💻 Autor
Autor: Alberto Agredano
Fecha: 17/10/2025
Asignatura: Programación Multimedia y Dispositivos Móviles
Proyecto académico Android Studio (Kotlin)
📜 Licencia
Este proyecto se ha desarrollado con fines educativos. Puedes usarlo, modificarlo o mejorarlo libremente con fines de aprendizaje.
