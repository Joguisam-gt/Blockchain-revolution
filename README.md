# Blockchain Revolution

Sitio web educativo e informativo sobre la tecnologia Blockchain y las Finanzas Descentralizadas (DeFi). Desarrollado para explicar de forma visual y accesible como funciona la cadena de bloques, sus ventajas y el ecosistema de criptomonedas.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

---

## Tecnologias utilizadas

Este proyecto fue desarrollado utilizando las siguientes tecnologias:

- **Lenguaje principal:** HTML5
- **Estilos:** CSS3 con Flexbox, Grid y animaciones personalizadas
- **Tipografia:** Google Fonts
- **Iconografia:** FontAwesome / Lucide Icons
- **Control de versiones:** Git y GitHub

---

# Como montar el proyecto

## Requisitos previos

Antes de ejecutar el proyecto, asegurate de tener instaladas las siguientes herramientas:

- [Git](https://git-scm.com/)
- Un servidor local que soporte rutas absolutas (recomendado: [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) para VS Code)
- [Visual Studio Code](https://code.visualstudio.com/) u otro editor de codigo

> **Importante:** El proyecto usa rutas absolutas (`/CSS/`, `/Pages/`, `/images/`). Debes servirlo desde un servidor local desde la raiz del proyecto. No funciona correctamente abriendo los archivos HTML directamente desde el sistema de archivos (`file://`).

Puedes comprobar las versiones instaladas con los siguientes comandos:

```bash
git --version
```

## 1. Clonar el repositorio

```bash
git clone https://github.com/usuario/Blockchain-revolution.git
```

## 2. Entrar a la carpeta del proyecto

```bash
cd Blockchain-revolution
```

## 3. Iniciar un servidor local

**Opcion A: Con VS Code + Live Server**

1. Abre la carpeta en VS Code.
2. Haz clic derecho sobre `index.html`.
3. Selecciona **"Open with Live Server"**.

**Opcion B: Con http-server (Node.js)**

```bash
npm install -g http-server
http-server . -p 8080
```

El proyecto estara disponible en:

```
http://localhost:8080
```

> No se requiere configuracion de variables de entorno. El proyecto no tiene backend ni base de datos.

---

# Estructura del proyecto

```text
Blockchain-revolution/
├── index.html                   # Pagina principal (landing page)
├── Pages/                       # Paginas internas del sitio
│   ├── Como-funciona.html       # Explicacion del funcionamiento de Blockchain
│   ├── Ventajas-defi.html       # Ventajas de las Finanzas Descentralizadas
│   └── Criptomonedas.html       # Informacion sobre criptomonedas principales
├── CSS/                         # Hojas de estilo
│   └── stylesheet.css           # Estilos globales del sitio
├── images/                      # Recursos visuales
│   ├── favicon/                 # Iconos del sitio para distintos dispositivos
│   ├── fondos/                  # Imagenes de fondo
│   └── iconos/                  # Iconos adicionales
└── README.md                    # Documentacion principal
```

## Descripcion de carpetas importantes

| Carpeta | Descripcion |
|---|---|
| `Pages/` | Contiene las paginas secundarias del sitio, una por tema. |
| `CSS/` | Hoja de estilos global que aplica a todas las paginas. |
| `images/` | Todos los recursos visuales: imagenes, fondos e iconos. |

---

# Documentacion del proyecto

## Descripcion general

Blockchain Revolution es un sitio web educativo e informativo que explica de manera clara y visual la tecnologia Blockchain y su impacto en las finanzas modernas a traves de DeFi (Finanzas Descentralizadas). El sitio esta orientado a usuarios que quieren entender este ecosistema sin conocimientos tecnicos previos.

## Objetivo general

Desarrollar un sitio web estatico, rapido y visualmente atractivo que divulgue los conceptos fundamentales de Blockchain, DeFi y criptomonedas utilizando unicamente HTML5 y CSS3.

## Objetivos especificos

- Presentar la tecnologia Blockchain de forma accesible y visual.
- Explicar el funcionamiento de las transacciones descentralizadas.
- Destacar las ventajas de DeFi frente a las finanzas tradicionales.
- Proporcionar informacion sobre las principales criptomonedas del mercado.
- Garantizar una experiencia responsive adaptada a cualquier dispositivo.

## Funcionalidades

El sistema permite realizar las siguientes acciones:

- Explorar la pagina principal con informacion introductoria sobre Blockchain y DeFi.
- Navegar a la seccion "Como funciona" para entender el mecanismo de la cadena de bloques.
- Consultar las ventajas de DeFi frente a las finanzas tradicionales.
- Revisar informacion sobre las principales criptomonedas del mercado.
- Acceder a enlaces externos a Binance Academy para aprender mas.
- Contactar a traves del formulario de contacto en la pagina principal.

## Usuarios del sistema

| Tipo de usuario | Permisos |
|---|---|
| Visitante | Puede navegar libremente por todas las paginas del sitio, consultar el contenido educativo y acceder a los enlaces externos. |

## Flujo principal

1. El usuario ingresa a la pagina principal (`index.html`).
2. Explora la seccion hero con la propuesta de valor del sitio.
3. Navega por las secciones de la pagina principal: Blockchain, DeFi y caracteristicas.
4. Usa el menu de navegacion para acceder a las paginas internas.
5. Consulta "Como funciona", "Ventajas DeFi" o "Criptomonedas" segun su interes.
6. Puede acceder a recursos externos (Binance Academy) o al formulario de contacto.

## Arquitectura

El proyecto utiliza una arquitectura de **sitio web estatico de multiples paginas**:

- **Sin backend:** Todo el contenido es estatico, servido directamente por el servidor local o un hosting estatico.
- **Sin base de datos:** No se almacena ni procesa informacion del usuario.
- **CSS global:** Un unico archivo `stylesheet.css` gestiona los estilos de todas las paginas.
- **Navegacion por rutas absolutas:** Las paginas se enlazan usando rutas desde la raiz del proyecto.

## Paginas del sitio

| Pagina | Ruta | Descripcion |
|---|---|---|
| Inicio | `/index.html` | Landing page principal con hero, seccion DeFi y caracteristicas de Blockchain. |
| Como funciona | `/Pages/Como-funciona.html` | Explicacion del mecanismo de Blockchain: bloques, cadenas y consenso. |
| Ventajas DeFi | `/Pages/Ventajas-defi.html` | Comparativa entre DeFi y las finanzas tradicionales. |
| Criptomonedas | `/Pages/Criptomonedas.html` | Informacion sobre Bitcoin, Ethereum, Cardano y otras criptomonedas. |

## Convenciones de codigo

Para mantener el proyecto organizado:

- Los nombres de clases CSS utilizan la convencion **BEM** (`bloque__elemento--modificador`).
- Cada pagina HTML contiene etiquetas semanticas (`<nav>`, `<section>`, `<footer>`).
- Las rutas de recursos usan rutas absolutas desde la raiz (`/CSS/`, `/Pages/`, `/images/`).
- No se utiliza JavaScript ni ninguna libreria externa de scripts.

## Convencion de commits

Utiliza mensajes claros y descriptivos:

```text
feat: agregar seccion de criptomonedas
fix: corregir responsive del navbar en mobile
docs: actualizar README con estructura del proyecto
style: ajustar colores de la seccion hero
refactor: reorganizar estilos del footer
```

## Capturas de pantalla

### Pagina principal

![Pagina principal](docs/images/pagina-principal.png)

### Pagina Como funciona

![Como funciona](docs/images/como-funciona.png)

> Guarda las capturas dentro de `docs/images/` y actualiza las rutas anteriores.

## Despliegue

El proyecto se puede desplegar en cualquier servicio de hosting estatico:

- **Recomendado:** [Vercel](https://vercel.com) o [Netlify](https://netlify.com) (arrastrar la carpeta del proyecto).
- **Alternativa:** GitHub Pages (configurar para servir desde la raiz del repositorio `main`).

## Problemas conocidos

- Las rutas absolutas (`/CSS/`, `/Pages/`, `/images/`) requieren un servidor local para funcionar. Abrir el archivo `index.html` directamente desde el explorador de archivos no cargara los estilos ni las paginas correctamente.
- No hay formulario de contacto funcional implementado; el boton de contacto redirige a un ancla en la pagina.

## Mejoras futuras

- Agregar animaciones de entrada con JavaScript para mejorar la experiencia visual.
- Implementar un formulario de contacto funcional con un servicio como Formspree o EmailJS.
- Agregar una seccion de glosario con terminos clave de Blockchain y DeFi.
- Incluir un modo claro (light mode) adicional al tema oscuro actual.

## Como contribuir

1. Crea un fork del repositorio.
2. Crea una nueva rama:

```bash
git checkout -b feature/nombre-funcionalidad
```

3. Realiza los cambios.
4. Guarda los cambios:

```bash
git add .
git commit -m "feat: agregar nueva funcionalidad"
```

5. Envia la rama a GitHub:

```bash
git push origin feature/nombre-funcionalidad
```

6. Crea un Pull Request.

## Autor

- **Nombre:** Jose Guillermo Rodriguez Samcam
- **GitHub:** [\[Enlace al perfil de GitHub\]](https://github.com/Joguisam-gt/Blockchain-revolution.git)

## Licencia

Este proyecto fue desarrollado con fines educativos.

---

## Lista de verificacion antes de entregar

- [x] El nombre y la descripcion del proyecto estan completos.
- [x] Las tecnologias utilizadas estan actualizadas.
- [x] Las instrucciones de instalacion funcionan.
- [x] No se requieren variables de entorno (proyecto 100% estatico).
- [x] La estructura corresponde al proyecto real.
- [x] Las funcionalidades estan descritas.
- [x] Las paginas del sitio estan documentadas.
- [x] El flujo de navegacion esta descrito.
- [x] Las capturas de pantalla tienen su seccion (pendiente de imagenes).
- [x] No se incluyeron contrasenas ni datos privados en el repositorio.
- [ ] Los datos del autor estan completos (completar carne, curso, seccion y correo).
- [ ] Las capturas de pantalla estan guardadas en `docs/images/`.
- [ ] Los enlaces de despliegue estan actualizados con la URL real del sitio.
