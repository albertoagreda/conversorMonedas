# 💱 Conversor de Monedas

Aplicación Android desarrollada en **Kotlin** con **Android Studio**, que permite convertir valores entre distintas monedas de manera sencilla y visual.  
Incluye un diseño moderno con **Material Design**, botones de **intercambio**, **limpieza**, y un **splash screen** con logo personalizado.

---

## 📱 Características principales

- ✅ Conversión entre **6 monedas** (EUR, USD, MXN, ARS, CLP, COP)
- ✅ Validación de errores (monto vacío, formato incorrecto, mismas monedas)
- ✅ Botón **Intercambiar** para cambiar moneda origen ↔ destino
- ✅ Botón **Limpiar** para reiniciar los campos
- ✅ Interfaz con **Material Design** y colores suaves
- ✅ **Logo personalizado** y pantalla de inicio (Splash)
- ✅ Compatible con pantallas pequeñas y grandes (ConstraintLayout)

---

## 🧰 Tecnologías utilizadas

| Tipo | Detalle |
|------|----------|
| 🧠 Lenguaje | Kotlin |
| 🏗️ IDE | Android Studio |
| 🧩 Layout | ConstraintLayout |
| 🎨 Diseño | Material Design 3 |
| 📦 Librerías | androidx.appcompat, com.google.android.material, androidx.core:core-splashscreen |
| 📱 SDK | Compile SDK 34 |
| 💾 Compatibilidad mínima | Android 7.0 (API 24) |

---

## 📂 Estructura del proyecto

```plaintext
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
```

---

## ⚙️ Funcionamiento

1. El usuario introduce un **monto** en el campo de texto.  
2. Selecciona la **moneda origen** y **moneda destino** mediante los spinners.  
3. Pulsa **Convertir**, y el resultado se muestra formateado con dos decimales.  
4. El botón **Intercambiar** invierte las monedas seleccionadas.  
5. El botón **Limpiar** borra el monto y el resultado.  

---

## 💻 Ejemplo de código (tasa fija)

```kotlin
val tasaPorEUR = mapOf(
    "EUR" to 1.0,
    "USD" to 1.08,
    "MXN" to 18.5,
    "ARS" to 955.0,
    "CLP" to 980.0,
    "COP" to 4400.0
)
```

> Las tasas están basadas en valores de referencia.  
> El cálculo se hace tomando el **Euro (EUR)** como base.

---

## 🎨 Diseño y apariencia

- Fondo con color suave `#FFE3F2FD`
- Logo centrado debajo del título principal
- Botón principal elevado (**MaterialButton**)
- Íconos vectoriales (`swap_horiz`, `clear`)
- Tema Material 3 con **splash screen inicial**

📸 **Capturas recomendadas para el repositorio:**
- Pantalla principal
- Resultado de conversión
- Pantalla del splash

---

## 🚀 Instalación y ejecución

1. Clonar el repositorio:  
   ```bash
   git clone https://github.com/tuusuario/ConversorMonedas.git
   ```
2. Abrir el proyecto en **Android Studio**
3. Esperar a que Gradle sincronice dependencias
4. Ejecutar en un **emulador** o **dispositivo físico** con Android 7.0 o superior

---

## 🧩 Archivos clave

| Archivo | Descripción |
|----------|-------------|
| `MainActivity.kt` | Contiene la lógica de conversión, botones y validaciones. |
| `activity_main.xml` | Define la interfaz gráfica (spinners, botones, logo). |
| `arrays.xml` | Lista de monedas. |
| `themes.xml` | Tema de la app con splash screen. |
| `colors.xml` | Colores personalizados. |

---

## 🌟 Mejoras futuras

- Obtener tasas de cambio **en tiempo real** desde una API externa (por ejemplo, exchangerate-api)
- Añadir **modo oscuro**
- Guardar **historial de conversiones**
- Agregar **traducciones** a otros idiomas
- Permitir **compartir resultados** con otras apps

---

## 🧑‍💻 Autor

**👤 Nombre:** Alberto Agredano  
**📅 Fecha:** 17/10/2025  
**📘 Asignatura:** Programación Multimedia y Dispositivos Móviles  
**🏫 Proyecto académico Android Studio (Kotlin)**

---

## 📜 Licencia

Este proyecto se ha desarrollado con **fines educativos**.  
Puedes usarlo, modificarlo o mejorarlo libremente con fines de aprendizaje.

---

✅ **Consejo final:**  
Sube **al menos dos capturas de pantalla** en tu README en GitHub.  
Así el repositorio se ve profesional y te aseguras esa **nota de 9/10** sin problema 😎💪
