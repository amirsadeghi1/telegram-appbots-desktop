

# 🚀 Ejecuta AppBots de Telegram (Juegos) en Escritorio – *Método de Bypass*

> 💡 Desbloquea **Juegos y Apps de Telegram** en Telegram Desktop usando un háck inteligente de inyección de scripts a nivel del navegador.  
> 🧠 Sin extensiones, sin modding: pura magia de DevTools.

![badge](https://img.shields.io/badge/Status-Stable-green)  
![badge](https://img.shields.io/github/stars/amirsadeghi1/telegram-appbots-desktop?style=social)  

---

## 🛠️ Rápido — Paso a paso

> ⏱ Tiempo estimado: 2–5 minutos

1. **Consigue el script**  
   Descarga o abre el archivo raw:  
   [`telegram-web-app.js`](https://raw.githubusercontent.com/amirsadeghi1/telegram-appbots-desktop/master/telegram-web-app.js)  
   O simplemente copia su contenido (`Ctrl+A`, `Ctrl+C`).

2. **Abre Telegram Desktop o Telegram Web**  
   Navega hasta el bot/juego que quieras iniciar.

3. **Inicia el bot y detente en el QR**  
   Haz clic en **Play**. Cuando aparezca el QR o el prompt de inicio de sesión, **no** lo escanees todavía: déjalo visible.

4. **Abre las Developer Tools**  
   Presiona `Ctrl+Shift+I` o `F12` para abrir DevTools.

5. **Ve a la pestaña “Sources”**

6. **Localiza `telegram-web-app.js`**  
   En la barra lateral izquierda, expande la carpeta `js` (o equivalente) → abre `telegram-web-app.js`.

7. **Reemplaza el contenido del archivo**  
   - Selecciona todo (`Ctrl+A`)  
   - Elimina  
   - Pega tu script copiado

8. **Habilita Overrides (crítico)**  
   - Haz clic derecho en el editor → **Override content**  
   - Haz clic en **Select folder** → elige o crea una (por ejemplo, `telegram-injector`)

9. **Concede permiso**  
   Cuando se te solicite, haz clic en **Allow**.

10. **Actualiza la página**  
    Presiona `Ctrl+R`.  
    🕹️ El bot/juego ahora debería **ejecutarse sin problemas** en el escritorio.

11. **Dale estrella al repositorio 💖**  
    Si esto te ahorró tiempo de ingeniería inversa, dale estrella aquí → [GitHub Repo](https://github.com/amirsadeghi1/telegram-appbots-desktop)

---

## ❗ Notas y solución de problemas
- Funciona mejor con navegadores basados en Chromium y Telegram Desktop (Electron).  
- Si el archivo se restablece tras recargar, asegúrate de que **Overrides** esté habilitado y que la carpeta tenga permisos de escritura.  
- Si sigue fallando, borra la caché o reinicia DevTools después de reemplazar el archivo.

---

## 🔒 Descargo de responsabilidad
Esta técnica modifica temporalmente archivos del lado del cliente en tiempo de ejecución.  
Úsalo responsablemente: solo en cuentas o bots que te pertenezcan o para los que tengas permiso para probarlos.
