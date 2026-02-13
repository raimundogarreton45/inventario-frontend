# 🚀 Cómo Subir Tu Interfaz a Internet (GRATIS)

## ✅ Lo Que Tienes Ahora

3 archivos HTML listos para usar:
1. **index.html** - Página de login
2. **dashboard.html** - Dashboard principal
3. **productos.html** - Gestión de productos

---

## 🎯 Opción 1: Vercel (RECOMENDADA - Más Fácil)

### Paso 1: Crear Cuenta en Vercel

1. Ve a https://vercel.com
2. Click **"Sign Up"**
3. Elige **"Continue with GitHub"**
4. Autoriza Vercel

### Paso 2: Preparar Archivos

1. **Descarga** los 3 archivos HTML (están en el ZIP)
2. Ponlos en una carpeta llamada `inventario-frontend`
3. Estructura:
   ```
   inventario-frontend/
   ├── index.html
   ├── dashboard.html
   └── productos.html
   ```

### Paso 3: Subir a GitHub

**Opción A: Si sabes usar Git:**

```bash
cd inventario-frontend
git init
git add .
git commit -m "Frontend inicial"
git remote add origin https://github.com/TU-USUARIO/inventario-frontend.git
git push -u origin main
```

**Opción B: Subir directo en GitHub.com:**

1. Ve a https://github.com/new
2. Repository name: `inventario-frontend`
3. Click **"Create repository"**
4. Click **"uploading an existing file"**
5. Arrastra los 3 archivos HTML
6. Click **"Commit changes"**

### Paso 4: Deploy en Vercel

1. Ve a https://vercel.com/new
2. Click **"Import Git Repository"**
3. Selecciona tu repo `inventario-frontend`
4. Click **"Import"**
5. **Framework Preset:** Deja en "Other"
6. Click **"Deploy"**

**¡Listo!** Vercel te da una URL como:
```
https://inventario-frontend.vercel.app
```

### Paso 5: Probar

Abre tu URL de Vercel:
- Deberías ver la página de login
- Inicia sesión con tus credenciales
- Todo debería funcionar conectado a tu API

---

## 🎯 Opción 2: Netlify (Alternativa)

### Paso 1: Crear Cuenta

1. Ve a https://netlify.com
2. **Sign up** con GitHub

### Paso 2: Deploy Manual (SIN GitHub)

1. En Netlify, ve a **Sites**
2. Arrastra la carpeta `inventario-frontend` al área de "Drag and drop"
3. **¡Listo!** Te da una URL como:
   ```
   https://random-name-123.netlify.app
   ```

### Cambiar el Nombre:

1. Site settings → Site information → Change site name
2. Pon: `inventario-pyme`
3. Tu URL será: `https://inventario-pyme.netlify.app`

---

## 🎯 Opción 3: GitHub Pages (MÁS Simple)

### Paso 1: Subir a GitHub

1. Crea repo `inventario-frontend` en GitHub
2. Sube los 3 archivos HTML

### Paso 2: Activar GitHub Pages

1. Repo → Settings → Pages
2. Source: **Deploy from a branch**
3. Branch: **main** → Folder: **/ (root)**
4. Click **Save**

Espera 1-2 minutos, tu URL será:
```
https://TU-USUARIO.github.io/inventario-frontend
```

---

## ✅ Verificar que Funciona

### Test 1: Login

1. Abre tu URL pública
2. Deberías ver la página de login bonita
3. Ingresa email y password de un usuario

### Test 2: Dashboard

1. Después del login, deberías ver:
   - Estadísticas (total productos, stock bajo)
   - Lista de productos
   - Formulario de ventas

### Test 3: Agregar Producto

1. Click en "+ Agregar" o ve a productos.html
2. Completa el formulario
3. Click "Agregar Producto"
4. Debería aparecer en la lista

---

## 🔧 Si Algo No Funciona

### Error: "API not responding"

**Causa:** Tu API de Railway está apagada o la URL cambió

**Solución:**
1. Verifica que Railway esté online
2. En cada archivo HTML, busca:
   ```javascript
   const API_URL = 'https://api-inventarioo-production.up.railway.app';
   ```
3. Verifica que sea TU URL de Railway
4. Si cambió, actualiza en los 3 archivos

### Error: CORS

**Causa:** Railway no permite peticiones desde tu dominio

**Solución:**
Ya está configurado en tu API, pero si da error, avísame.

### Error: "Cannot read properties"

**Causa:** Respuesta inesperada de la API

**Solución:**
1. Abre la consola del navegador (F12)
2. Ve a "Console"
3. Mándame el error exacto

---

## 🎨 Personalizar Dominio (Opcional)

### En Vercel:

1. Settings → Domains
2. Add Domain
3. Sigue instrucciones para configurar DNS

### Ejemplo:
Tu URL podría ser: `inventario.tuempresa.cl`

**Costo:** $0 si tienes dominio, o ~$10.000/año por dominio nuevo

---

## 📱 Hacer PWA (App Móvil)

Los clientes pueden agregar tu web a su pantalla de inicio:

### Android:
1. Abre la URL en Chrome
2. Menu → "Agregar a pantalla de inicio"

### iOS:
1. Abre la URL en Safari
2. Botón compartir → "Agregar a inicio"

Se verá como una app nativa.

---

## 🔐 URLs Finales para Dar a Clientes

**Login (pública):**
```
https://tu-frontend.vercel.app
```

**Dashboard (protegida, solo después de login):**
```
https://tu-frontend.vercel.app/dashboard.html
```

**Productos (protegida):**
```
https://tu-frontend.vercel.app/productos.html
```

---

## 💰 Costos

| Servicio | Costo |
|----------|-------|
| Vercel | $0/mes |
| Netlify | $0/mes |
| GitHub Pages | $0/mes |
| **TOTAL** | **$0/mes** |

**Límites gratuitos:**
- Vercel: 100 GB bandwidth/mes
- Netlify: 100 GB bandwidth/mes
- GitHub Pages: 100 GB bandwidth/mes

**Suficiente para:** 10,000-50,000 usuarios/mes

---

## ✅ Checklist de Deploy

- [ ] Archivos HTML descargados
- [ ] Repositorio en GitHub creado
- [ ] Archivos subidos a GitHub
- [ ] Deploy en Vercel/Netlify completado
- [ ] URL pública funciona
- [ ] Login funciona
- [ ] Dashboard carga productos
- [ ] Se pueden registrar ventas
- [ ] Se pueden agregar productos

---

## 🎯 Siguiente Paso

Una vez online:

1. **Crea una cuenta demo:**
   - Email: demo@ejemplo.cl
   - Password: demo123
   - Agrega 5-10 productos

2. **Guarda tu URL:**
   ```
   https://inventario-pyme.vercel.app
   ```

3. **Usa esa URL para vender:**
   - Muéstrala en tu celular
   - Comparte por WhatsApp
   - Post en redes sociales

---

## 📞 Para Vender

**Tu pitch:**

> "Mira, este es tu sistema de inventario:
> 
> [Abres tu URL en el celular]
> 
> Entras con tu email y listo.
> 
> Aquí ves todos tus productos, registras ventas, y te llegan alertas cuando algo se está acabando.
> 
> ¿Quieres probarlo? Te creo la cuenta ahora mismo."

---

## 🆘 Ayuda

Si algo no funciona:
1. Verifica logs de la API en Railway
2. Verifica consola del navegador (F12)
3. Asegúrate que la URL de la API sea correcta en los HTML

---

**¡Tu interfaz profesional está lista para vender! 🎉**
