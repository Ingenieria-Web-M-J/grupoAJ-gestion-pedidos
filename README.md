# Sistema de Inventarios de Pedidos

Este proyecto es una aplicación de gestión de inventario de materiales desarrollada con Next.js y React en el frontend, Prisma como ORM para la gestión de la base de datos y Auth0 para la autenticación. La aplicación permite a los usuarios administrar entradas y salidas de materiales y gestionar roles de usuario.

## Integrantes

- Arley Santiago Tangarife Velasquez
- Jose Luis Aguirre Ramirez

## Usuarios de prueba

ADMIN: adminingeweb@udea.edu.co
USER: useringeweb@udea.edu.co

Contraseña para ambas cuentas: Ingeweb2024

## Características

- **Autenticación**: Integración con Auth0 para manejar el inicio de sesión y la gestión de usuarios.
- **Roles de Usuario**:
  - **Administrador**: Puede generar entradas y salidas de material, así como cambiar roles de usuario.
  - **Usuario Genérico**: Puede agregar nuevos materiales al inventario.
- **Base de Datos**: Gestión eficiente de la base de datos utilizando Prisma.

## Tecnologías Utilizadas

- **Next.js**: Framework de React para la creación de aplicaciones web.
- **React**: Biblioteca para construir interfaces de usuario.
- **Prisma**: ORM (Object-Relational Mapping) para la gestión de la base de datos.
- **Auth0**: Plataforma de autenticación y autorización.

## Requisitos Previos

Antes de comenzar, asegúrate de tener instalado:

- Node.js (versión 14 o superior)
- npm (versión 6 o superior) o Yarn

## Instalación

1. **Clonar el repositorio**:

   ```bash
   git clone https://github.com/tu-usuario/sistema-inventarios.git
   cd sistema-inventarios
   ```

2. **Instalar las dependencias**:

   ```bash
   npm install
   # o
   yarn install
   ```

3. **Configurar las variables de entorno**:

   Crea un archivo `.env` en la raíz del proyecto y añade las siguientes variables:

   ```env
   DATABASE_URL=postgresql://usuario:contraseña@localhost:5432/nombre_base_datos
   AUTH0_DOMAIN=tu-dominio.auth0.com
   AUTH0_CLIENT_ID=tu-client-id
   AUTH0_CLIENT_SECRET=tu-client-secret
   NEXTAUTH_URL=http://localhost:3000
   NEXTAUTH_SECRET=your-nextauth-secret
   ```

4. **Configurar Prisma**:

   Genera el cliente de Prisma:

   ```bash
   npx prisma generate
   ```

   Si necesitas migrar el esquema de la base de datos:

   ```bash
   npx prisma migrate dev --name init
   ```

## Uso

1. **Iniciar el servidor de desarrollo**:

   ```bash
   npm run dev
   # o
   yarn dev
   ```

   La aplicación estará disponible en `http://localhost:3000`.

## Funcionalidades

### Administrador

- **Generar Entradas y Salidas de Material**: El administrador puede agregar y retirar materiales del inventario.
- **Cambiar Roles de Usuario**: El administrador puede asignar roles a los usuarios, promoviendo o degradando sus permisos.

### Usuario Genérico

- **Agregar Materiales**: El usuario genérico puede agregar nuevos materiales al inventario.

## Estructura del Proyecto

- **pages/**: Contiene las rutas y páginas de Next.js.
- **components/**: Componentes reutilizables de React.
- **lib/**: Utilidades y configuraciones globales.
- **prisma/**: Esquema y cliente de Prisma.
- **styles/**: Archivos de estilos CSS y SASS.

## Contribución

Las contribuciones son bienvenidas. Puedes hacer un fork del repositorio y crear una pull request con tus mejoras o correcciones.

## Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.

---

Si necesitas más detalles o tienes alguna pregunta, no dudes en contactarme.

