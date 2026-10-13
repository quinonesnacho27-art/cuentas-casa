# Cuentas de la Casa

Página para anotar los gastos e ingresos de la casa y el camión día a día, ver en qué se va la plata cada mes, comparar meses y seguir las deudas en cuotas.

- Funciona en el celular y en el computador (se puede agregar a la pantalla de inicio).
- Los datos se guardan en Firebase (Firestore) y se sincronizan entre todos los que tienen acceso.
- Se entra con una cuenta de Google. Solo los correos autorizados por el dueño pueden ver y anotar.
- Sin internet se puede seguir anotando: se sube solo cuando vuelve la conexión.

## Archivos

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La aplicación completa |
| `firebase-config.js` | Datos públicos del proyecto de Firebase |
| `manifest.webmanifest`, `icon-*.png`, `icon.svg` | Para instalarla como app en el celular |
| `sw.js` | Permite abrirla aunque no haya internet |

Este repositorio **no contiene datos de gastos**. Los datos viven solo en la base de datos de Firebase, protegida por reglas que exigen iniciar sesión con un correo autorizado.

## Dar acceso a alguien

1. Entra a la página con la cuenta del dueño.
2. Ve a **Categorías → Personas con acceso** y agrega su correo de Google.
3. Envíale el enlace de la página. Debe entrar con ese mismo correo.
