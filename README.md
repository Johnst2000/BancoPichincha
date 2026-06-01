# Diseño Responsivo del Inicio de Sesión — Banco Pichincha

Proyecto académico del curso **Aplicaciones Móviles** (6.º semestre). Réplica educativa de la pantalla de inicio de sesión de **Banco Pichincha**, enfocada en diseño responsivo, maquetación en XML y uso de recursos gráficos en Android.

## Descripción

La aplicación muestra una interfaz de login fiel al diseño de referencia del banco: header con logo, ilustración hero, slogan de seguridad, tarjetas de métodos de autenticación, accesos rápidos y pie de pantalla. El layout se adapta a distintos tamaños de pantalla mediante `NestedScrollView` y `ConstraintLayout`. Es una entrega de **interfaz estática** (sin lógica de autenticación ni navegación).

## Stack tecnológico

| Tecnología | Uso |
|------------|-----|
| **Kotlin** | `MainActivity.kt` — actividad principal |
| **XML** | Layouts, drawables, colores, dimensiones y cadenas |
| **Android SDK** | Material Components, vistas del framework |
| **Android Studio** | Desarrollo, compilación y ejecución en emulador o dispositivo |

## Entregable principal

El archivo central de la entrega es el layout:

`app/src/main/res/layout/activity_main.xml`

Define la estructura visual completa de la pantalla de login (header, hero, tarjetas, utilidades y footer).

## Características

- Layout responsive con `NestedScrollView` + `ConstraintLayout`
- Header con logo completo (PNG)
- Ilustración hero (PNG)
- Slogan de seguridad
- Tres tarjetas de acceso: usuario/contraseña, huella/Face ID, PIN de 6 dígitos
- Accesos rápidos: Ubícanos, Clave digital, Llámanos
- Enlace inferior: ¿Ingresar con otro usuario?
- Barra de estado clara sobre fondo blanco

## Paleta de colores

| Uso              | Color     | Hex       |
|------------------|-----------|-----------|
| Fondo            | Blanco    | `#FFFFFF` |
| Logo / acento    | Amarillo  | `#FFD100` |
| Texto principal  | Azul oscuro | `#002855` |
| Enlaces / íconos | Azul secundario | `#0066CC` |
| Versión          | Gris      | `#757575` |

## Estructura del proyecto

```
app/src/main/
├── java/com/example/bancopichincha/
│   └── MainActivity.kt
└── res/
    ├── drawable/
    │   ├── bg_login_card.xml          (forma de tarjeta — XML)
    │   ├── ic_logo_bp.png             (logo header)
    │   ├── imagen_bp.png              (ilustración hero)
    │   ├── ic_usuario.png             (tarjeta usuario)
    │   ├── ic_huella.png              (tarjeta huella)
    │   ├── ic_pin.png                 (tarjeta PIN)
    │   ├── ic_ubicacion.png           (utilidad ubicación)
    │   ├── ic_llave.png               (utilidad clave digital)
    │   └── ic_celular.png             (utilidad llamada)
    ├── layout/
    │   └── activity_main.xml
    └── values/
        ├── colors.xml
        ├── dimens.xml
        ├── strings.xml
        └── styles.xml
```

## Assets PNG (`drawable/`)

Coloca tus imágenes PNG en `app/src/main/res/drawable/` con estos nombres exactos:

| Archivo           | Uso en pantalla              |
|-------------------|------------------------------|
| `ic_logo_bp.png`  | Logo completo del header     |
| `imagen_bp.png`   | Ilustración hero             |
| `ic_usuario.png`  | Ícono tarjeta usuario        |
| `ic_huella.png`   | Ícono tarjeta huella         |
| `ic_pin.png`      | Ícono tarjeta PIN            |
| `ic_ubicacion.png`| Ícono Ubícanos               |
| `ic_llave.png`    | Ícono Clave digital          |
| `ic_celular.png`  | Ícono Llámanos               |

El layout (`activity_main.xml`) ya referencia estos drawables. Solo reemplaza o añade los PNG en la carpeta indicada.

## Requisitos

- Android Studio (Ladybug o superior recomendado)
- minSdk 34, targetSdk 36
- Kotlin + Material Components

## Cómo ejecutar

1. Abre el proyecto en **Android Studio**.
2. Sincroniza Gradle (Sync Project with Gradle Files).
3. Crea o selecciona un **emulador** Android (API 34+) o conecta un dispositivo físico con depuración USB.
4. Pulsa **Run** (▶) y verifica la pantalla de login en ejecución.

## Capturas de pantalla

Evidencia visual de la aplicación en ejecución y del diseño de referencia. Puedes:

- **Opción A:** Pegar las imágenes directamente en el editor de GitHub entre cada sección (debajo del encabezado).
- **Opción B:** Guardar los PNG en la carpeta `capturas/` del repositorio y descomentar las líneas `![...](capturas/...)`.

| Archivo sugerido | Contenido |
|------------------|-----------|
| `capturas/captura1.png` | Vista completa del login |
| `capturas/captura2.png` | Tarjetas de autenticación |
| `capturas/captura3.png` | Accesos rápidos y footer |
| `capturas/captura4.png` | Diseño de referencia de la app |

---

### Captura 1 — Vista completa de la pantalla de Login en ejecución

<!-- Pegar imagen aquí -->

![Captura 1](capturas/captura1.png)

*(insertar imagen aquí)*










---

### Captura 2 — Tarjetas de Autenticación en ejecución

<!-- Pegar imagen aquí -->

![Captura 2](capturas/captura2.png)

*(insertar imagen aquí)*










---

### Captura 3 — Accesos Rápidos y Footer en ejecución

<!-- Pegar imagen aquí -->

![Captura 3](capturas/captura3.png)

*(insertar imagen aquí)*










---

### Captura 4 — Captura del diseño de la App

<!-- Pegar imagen aquí -->

![Captura 4](capturas/captura4.png)

*(insertar imagen aquí)*










---

## Notas

- Los íconos e ilustraciones son PNG proporcionados por el usuario; no se incluyen vectores XML temporales.
- Las tarjetas y utilidades son solo UI; no tienen navegación ni lógica de autenticación implementada.
- Proyecto con fines educativos; no está afiliado a Banco Pichincha.
