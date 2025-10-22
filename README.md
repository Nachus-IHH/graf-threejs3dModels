Ignacio Hernandez Hernandez 23200144
# 🌐 GRAF-THREEJS3DMODELS

Proyecto que integra múltiples ejemplos de modelos 3D utilizando **Three.js**, centralizados en una sola página web accesible desde GitHub Pages.  
Permite visualizar modelos en distintos formatos (FBX, GLTF, Collada) mediante un selector interactivo, evitando cambiar manualmente la URL.

---

## 🎯 Objetivos del Proyecto

- **Unificar la visualización de modelos 3D** en una sola interfaz accesible desde una única página (`index.html`).
- **Explorar diferentes formatos 3D** compatibles con Three.js: Collada, GLTF y FBX.
- **Comprender el funcionamiento de distintos loaders** de Three.js.
- **Implementar una interfaz simple y funcional** para facilitar la navegación entre ejemplos.
- **Preparar el proyecto para despliegue en GitHub Pages** como demostración de modelos 3D.

---

## 🧩 Tecnologías Utilizadas

- **[Three.js](https://threejs.org/)** – Librería JavaScript para renderizado 3D en WebGL.  
- **HTML5 / CSS3 / JavaScript** – Estructura, estilo e interacción.  
- **WebGL** – API para renderizado gráfico acelerado por GPU.  
- **GitHub Pages** – Hospedaje del visor 3D de forma pública.

---

## ⚙️ Funcionamiento del `index.html`

El archivo principal (`index.html`) contiene un **selector desplegable** que permite elegir qué ejemplo cargar.  
Cada modelo se muestra dentro de un `<iframe>` sin necesidad de cambiar de página.

### Ejemplo del selector
```html
<select id="modelSelector">
  <option value="examples/webgl_loader_collada_kinematics.html">Collada Kinematics</option>
  <option value="examples/webgl_loader_collada_skinning.html">Collada Skinning</option>
  <option value="examples/webgl_loader_fbx.html">FBX</option>
  <option value="examples/webgl_loader_gltf_avif.html">GLTF Avif</option>
</select>
```
El cambio de modelo se realizara dinamicamente mediante:
viewer.src = selector.value;
