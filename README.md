# Diseño Responsivo del Inicio de Sesión — Banco Pichincha

Proyecto académico del curso **Aplicaciones Móviles** (6.º semestre). Réplica educativa de la pantalla de inicio de sesión de **Banco Pichincha**, enfocada en diseño responsivo, maquetación en XML y uso de recursos gráficos en Android.

## Descripción

La aplicación muestra una interfaz de login fiel al diseño de referencia del banco: header con logo, ilustración hero, slogan de seguridad, tarjetas de métodos de autenticación, accesos rápidos y pie de pantalla. El layout se adapta a distintos tamaños de pantalla mediante `NestedScrollView` y `ConstraintLayout`. Es una entrega de **interfaz estática** (sin lógica de autenticación ni navegación).

## Entregable principal

El archivo central de la entrega es el layout:

`app/src/main/res/layout/activity_main.xml`

Define la estructura visual completa de la pantalla de login (header, hero, tarjetas, utilidades y footer).

## Características

- Layout responsive
- Header con logo completo (PNG)
- Ilustración hero (PNG)
- Slogan de seguridad
- Tres tarjetas de acceso: usuario/contraseña, huella/Face ID, PIN de 6 dígitos
- Accesos rápidos: Ubícanos, Clave digital, Llámanos
- Enlace inferior: ¿Ingresar con otro usuario?

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
    └── layout/
        └── activity_main.xml

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


## Capturas de pantalla
### Captura 1 — Vista completa de la pantalla de Login en ejecución
<img width="382" height="730" alt="image" src="https://github.com/user-attachments/assets/fde869b4-eb99-4d98-95bb-644f8e4da516" />
---

### Captura 2 — Tarjetas de Autenticación en ejecución
<img width="584" height="196" alt="image" src="https://github.com/user-attachments/assets/b6b198e0-4756-4002-a4c4-8688911b1e17" />

---

### Captura 3 — Accesos Rápidos y Footer en ejecución
<img width="616" height="277" alt="image" src="https://github.com/user-attachments/assets/5a186d96-62da-411d-afaf-c80164708bc7" />

---

### Captura 4 — Captura del diseño de la App
<img width="1518" height="902" alt="image" src="https://github.com/user-attachments/assets/d99492d5-1e0c-40e9-bb98-a72ad3b7878d" />

---
