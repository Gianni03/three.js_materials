# Three.js Materials Demo

Este proyecto es una demostración interactiva de materiales en Three.js, enfocándose principalmente en el **`MeshPhysicalMaterial`** y sus capacidades avanzadas de renderizado realista.

## Características Principales

- **Materiales Físicos Avanzados**: Implementación de `MeshPhysicalMaterial` para demostrar propiedades como:
  - **Transmisión**: Efectos de vidrio y transparencia refractiva.
  - **Iridiscencia**: Efectos de interferencia de película delgada (como manchas de aceite o burbujas).
  - **Metalness & Roughness**: Control preciso sobre las propiedades metálicas y rugosidad de la superficie.
- **Iluminación HDR**: Uso de `RGBELoader` para cargar un mapa de entorno de alto rango dinámico (HDR) para una iluminación y reflejos realistas.
- **Interactividad**: Interfaz de usuario integrada con **`lil-gui`** para ajustar parámetros del material en tiempo real.
- **Geometrías**: Demostración sobre múltiples geometrías (Esfera, Plano, Torus).

## Tecnologías Utilizadas

- **[Three.js](https://threejs.org/)**: Biblioteca principal para gráficos 3D.
- **[Vite](https://vitejs.dev/)**: Entorno de desarrollo rápido y bundler.
- **[lil-gui](https://lil-gui.georgealways.com/)**: Biblioteca ligera para crear interfaces de control flotantes.

## Instalación y Uso

Asegúrate de tener [Node.js](https://nodejs.org/) instalado en tu sistema.

1. **Instalar dependencias**:

   ```bash
   npm install
   ```

   _(O `pnpm install` / `yarn install` si prefieres otros gestores de paquetes)_

2. **Ejecutar servidor de desarrollo**:

   ```bash
   npm run dev
   ```

3. **Abrir en el navegador**:
   El servidor iniciará típicamente en `http://localhost:5173`. Abre esa dirección para interactuar con la escena.

## Controles

- **Mouse / Touch**: Usa `OrbitControls` para rotar, hacer zoom y moverte alrededor de la escena.
- **Panel GUI**: Usa el panel en la esquina superior derecha para modificar las propiedades del material (`metalness`, `roughness`, `transmission`, etc.) y observar los cambios en tiempo real.
