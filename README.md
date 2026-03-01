VEGGIES MARKET

Plataforma de e-commerce para vender productos agrícolas directamente entre productores y clientes.


COMO FUNCIONA

Clientes:
- Acceden a la plataforma sin registrarse
- Ven el catálogo de productos disponibles
- Pueden buscar y filtrar por categoría
- Ven las ofertas de cada productor

Productores:
- Se registran en la plataforma
- Acceden a su panel personal
- Seleccionan productos del catálogo
- Añaden precio y cantidad disponible
- Sus ofertas aparecen en el catálogo público

Administrador:
- Gestiona usuarios (activa/desactiva)
- Verifica a los productores
- Crea y edita productos en el catálogo
- Gestiona categorías
- Ve todas las ofertas activas


INSTALACION

Requisitos:
- PHP 7.4 o superior
- MySQL 8.0 o superior
- Apache (AMPPS recomendado)

Pasos:

1. Descargar AMPPS desde www.ampps.com

2. Clonar el proyecto
   git clone https://github.com/veggiesmarket/veggies-market.git
   cd veggies-market-complete

3. Copiar a AMPPS
   Windows: C:\Program Files\Ampps\www\
   Mac/Linux: ~/ampps/www/

4. Crear base de datos
   - Abre phpMyAdmin en AMPPS
   - Crea base de datos: veggies_market
   - Importa: database/schema.sql

5. Configurar conexión
   - Edita config/config.php
   - Asegúrate de que los datos coincidan con tu MySQL

6. Acceder
   http://localhost/veggies-market-complete/


USUARIOS DE PRUEBA

Admin:      admin / 123456
Productor:  productor1 / 123456
Cliente:    cliente1 / 123456


ESTRUCTURA

app/
  controllers/    Lógica de la aplicación
  models/         Acceso a base de datos
  views/          Páginas HTML

config/
  config.php      Configuración

database/
  schema.sql      Estructura de BD

public/
  css/            Estilos
  js/             Scripts


TECNOLOGIAS

Backend:    PHP 7.4+
Base de datos: MySQL 8.0+
Frontend:   HTML5, CSS3, JavaScript
Patrón:     MVC


FUNCIONES PRINCIPALES

                    
Ver catálogo          Cliente SI       Productor SI      Admin SI

Buscar                Cliente SI       Productor SI      Admin SI

Añadir ofertas        Cliente NO       Productor SI      Admin NO

Crear productos       Cliente NO       Productor NO      Admin SI

Gestionar usuarios    Cliente NO       Productor NO      Admin SI

Gestionar categorías  Cliente NO       Productor NO      Admin SI


SEGURIDAD

- Contraseñas encriptadas
- Protección contra SQL injection
- Validación de sesiones
- Sanitización de datos


PROXIMAS VERSIONES

- Carrito de compras
- Pagos con Stripe
- Reseñas de productos
- Notificaciones por email


Versión: 1.0.0
Licencia: MIT
