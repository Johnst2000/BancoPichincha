# Banco Pichincha — Pantalla de Login (Android)

Réplica educativa de la pantalla de inicio de sesión de **Banco Pichincha** para el curso de Aplicaciones Móviles.

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

## Assets PNG (proporcionados por el usuario)

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

El layout (`activity_main.xml`) ya referencia estos drawables. Solo reemplaza los PNG en la carpeta indicada.

## Requisitos

- Android Studio (Ladybug o superior recomendado)
- minSdk 34, targetSdk 36
- Kotlin + Material Components

## Ejecución

1. Abre el proyecto en Android Studio.
2. Sincroniza Gradle.
3. Ejecuta en emulador o dispositivo físico (Run ▶).

## Notas

- Los íconos e ilustraciones son PNG proporcionados por el usuario; no se incluyen vectores XML temporales.
- Las tarjetas y utilidades son solo UI; no tienen navegación ni lógica de autenticación implementada.
