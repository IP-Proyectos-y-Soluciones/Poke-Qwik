# Poke-Qwik

**Descripción del Proyecto**

Este proyecto aprovecha el potencial de Qwik como framework principal y Tailwind como framework de CSS. En el README encontrarás información esencial para comprender y trabajar con el proyecto, incluyendo:

1. **¿Por qué un nuevo framework?**
   Explora las razones detrás de la elección de este framework, destacando sus ventajas y características distintivas.

2. **¿Qué es Qwik?**
   Ofrece una introducción a Qwik, explicando sus funcionalidades clave y cómo se integra en el proyecto.

3. **Estructura de Directorios**
   Proporciona una visión general de la organización de archivos y carpetas en el proyecto para facilitar la navegación y comprensión.

4. **Proyectos**
   Ofrece información sobre la gestión de proyectos dentro del framework, destacando las mejores prácticas y consideraciones.

5. **Introducción a:**
   - **Qwik**
     Brinda detalles esenciales sobre Qwik, resaltando su papel central en el desarrollo del proyecto.
   - **Qwik-City**
     Explora específicamente el subproyecto Qwik-City, proporcionando información detallada sobre su propósito y funcionalidades.

6. **Señales y Estados**
   Detalla el manejo de señales y estados en el contexto del proyecto, resaltando su importancia y aplicación.

7. **Rutas Básicas**
   Proporciona una guía sobre las rutas fundamentales dentro del proyecto, facilitando la navegación y comprensión del flujo de trabajo.

8. **Instalar Tailwind**
   Instrucciones claras sobre cómo integrar y configurar Tailwind como el framework de CSS, asegurando una presentación visual coherente.

9. **Carga Perezosa de Imágenes**
   Explica la implementación de la carga perezosa de imágenes en el proyecto, optimizando el rendimiento y la eficiencia.

10. **Eventos**
    Detalla cómo se manejan los eventos en el contexto del proyecto, proporcionando una comprensión clara de la interactividad.

11. **Serialización de Funciones**
    Explora la serialización de funciones, destacando su utilidad y aplicación específica en el proyecto.

Este README sirve como guía integral para entender y contribuir al proyecto, ofreciendo información detallada sobre su estructura, herramientas clave y mejores prácticas. ¡Bienvenido a la comunidad!

## Qwik City App ⚡️

- [Qwik Docs](https://qwik.builder.io/)
- [Discord](https://qwik.builder.io/chat)
- [Qwik GitHub](https://github.com/BuilderIO/qwik)
- [@QwikDev](https://twitter.com/QwikDev)
- [Vite](https://vitejs.dev/)

---

## Project Structure

This project is using Qwik with [QwikCity](https://qwik.builder.io/qwikcity/overview/). QwikCity is just an extra set of tools on top of Qwik to make it easier to build a full site, including directory-based routing, layouts, and more.

Inside your project, you'll see the following directory structure:

```bash
├── public/
│   └── ...
└── src/
    ├── components/
    │   └── ...
    └── routes/
        └── ...
```

- `src/routes`: Provides the directory-based routing, which can include a hierarchy of `layout.tsx` layout files, and an `index.tsx` file as the page. Additionally, `index.ts` files are endpoints. Please see the [routing docs](https://qwik.builder.io/qwikcity/routing/overview/) for more info.

- `src/components`: Recommended directory for components.

- `public`: Any static assets, like images, can be placed in the public directory. Please see the [Vite public directory](https://vitejs.dev/guide/assets.html#the-public-directory) for more info.

## Add Integrations and deployment

Use the `yarn qwik add` command to add additional integrations. Some examples of integrations includes: Cloudflare, Netlify or Express Server, and the [Static Site Generator (SSG)](https://qwik.builder.io/qwikcity/guides/static-site-generation/).

```shell
yarn qwik add # or `yarn qwik add`
```

## Development

Development mode uses [Vite's development server](https://vitejs.dev/). The `dev` command will server-side render (SSR) the output during development.

```shell
npm start # or `yarn start`
```

> Note: during dev mode, Vite may request a significant number of `.js` files. This does not represent a Qwik production build.

## Preview

The preview command will create a production build of the client modules, a production build of `src/entry.preview.tsx`, and run a local server. The preview server is only for convenience to preview a production build locally and should not be used as a production server.

```shell
yarn preview # or `yarn preview`
```

## Production

The production build will generate client and server modules by running both client and server build commands. The build command will use Typescript to run a type check on the source code.

```shell
yarn build # or `yarn build`
```
