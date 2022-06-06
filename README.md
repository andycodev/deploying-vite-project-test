# Vue 3 + Vite

This template should help get you started developing with Vue 3 in Vite. The template uses Vue 3 `<script setup>` SFCs, check out the [script setup docs](https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup) to learn more.

## Recommended IDE Setup

- [VS Code](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar)


### Deploying of Vite in GitHub Pages

1. Tener un proyecto vite creado

2. Crear un nuevo repositorio en su github 
* El nombre del respositorio será el nombre de la ruta

3. Subir proyecto vite al repositorio creado

4. Agregar la llave base al archivo vite.config.js que esta en la raiz del proyecto

export default defineConfig({
    base: '/nombre_repositorio/',               <----//línea agregada
    plugins: [vue()]
})

5. Compilamos nuestro proyecto vite para producció con el comando:
 npm run build

6. Agregamos nuestra carpeta build generada con el comando anterior a nuestro repositorio con el comando:
git add dist -f
git commit -m "adding dist"
git subtree push --prefix dist origin gh-pages

7. Listo, vamos a Settings de nuestro repositorio, luego en pages y abrimos la url.

Su página debería visualizarse en el navegador.

