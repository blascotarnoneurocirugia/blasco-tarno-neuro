# Instrucciones para subir a GitHub y GitHub Pages

## 1️⃣ Preparar el repositorio local

```bash
cd blasco-tarno-neuro
git init
git add .
git commit -m "Primera versión del sitio web Blasco Tarno Neurocirugía"
```

## 2️⃣ Crear repositorio en GitHub

1. Ve a https://github.com y haz login
2. Click en el botón "+" (arriba derecha) → "New repository"
3. Nombre del repositorio: `blasco-tarno-neuro` (o el que prefieras)
4. Descripción: "Sitio web oficial equipo neurocirugía Dr. Blasco / Dra. González Tarno"
5. Selecciona "Public" o "Private" según prefieras
6. **NO** marques "Initialize this repository with a README"
7. Click en "Create repository"

## 3️⃣ Conectar repositorio local con GitHub

Copia los comandos que GitHub te muestra (algo como esto, con tu usuario):

```bash
git remote add origin https://github.com/TU-USUARIO/blasco-tarno-neuro.git
git branch -M main
git push -u origin main
```

## 4️⃣ Activar GitHub Pages

1. En tu repositorio de GitHub, ve a **Settings** (arriba derecha)
2. En el menú izquierdo, click en **Pages**
3. En "Source", selecciona **main** branch
4. Click en **Save**
5. Espera unos minutos (GitHub te dirá la URL donde estará publicado)

Tu sitio estará disponible en: `https://TU-USUARIO.github.io/blasco-tarno-neuro/`

## 5️⃣ Dominio personalizado (opcional)

Si quieres usar tu propio dominio (ej: www.blascotarno.com):

1. En la configuración de GitHub Pages, añade tu dominio en "Custom domain"
2. En tu proveedor de dominios, configura:
   - Un registro **A** apuntando a las IPs de GitHub:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - Un registro **CNAME** de `www` apuntando a `TU-USUARIO.github.io`

## 🔄 Actualizar el sitio

Cuando quieras actualizar la web:

```bash
git add .
git commit -m "Descripción de los cambios"
git push
```

Los cambios aparecerán en la web en 1-2 minutos.

## 📝 Notas importantes

- El archivo `index.html` será la página principal
- Asegúrate de que todas las imágenes están en la carpeta `images/`
- Los enlaces entre páginas usan rutas relativas (ya configuradas)
- GitHub Pages es gratuito para repositorios públicos

## 🆘 Problemas comunes

**Las imágenes no se ven:**
- Verifica que están en la carpeta `images/`
- Verifica que los nombres coinciden exactamente (mayúsculas/minúsculas)

**Los cambios no aparecen:**
- Espera 2-3 minutos después del push
- Limpia la caché del navegador (Ctrl+Shift+R)

**Error 404:**
- Asegúrate de que el archivo `index.html` está en la raíz del repositorio
- Verifica que GitHub Pages está activado en Settings

---

¿Necesitas ayuda? Escribe a: ruberblascotarno@gmail.com
