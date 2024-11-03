# API de Reservas de Habitaciones de Hotel

Esta API REST permite gestionar las reservas de habitaciones en un hotel. Los clientes pueden buscar habitaciones disponibles y realizar reservas, mientras que los administradores pueden gestionar (añadir, editar o eliminar) las habitaciones.

## Tabla de Contenidos

- [Características](#características)
- [Requisitos Previos](#requisitos-previos)
- [Instalación](#instalación)
- [Configuración](#configuración)
- [Modelos](#modelos)
- [Endpoints](#endpoints)
- [Autenticación y Autorización](#autenticación-y-autorización)
- [Reglas de Negocio](#reglas-de-negocio)
- [Uso de Swagger](#uso-de-swagger)

## Características

- Gestión de habitaciones de hotel:
  - Crear, actualizar, eliminar habitaciones (solo administradores).
- Gestión de reservas de habitaciones:
  - Buscar y reservar habitaciones disponibles (solo clientes).
- Validación de reservas para evitar:
  - Reservas en fechas pasadas.
  - Reservas que duren más de 30 días.
- Autenticación basada en roles:
  - **Admin**: puede gestionar habitaciones.
  - **Customer**: puede realizar reservas.

## Requisitos Previos

- [.NET 6.0 SDK](https://dotnet.microsoft.com/download)
- [Entity Framework Core](https://docs.microsoft.com/en-us/ef/core/)
- SQL Server (u otra base de datos compatible)

## Instalación

1. Clona el repositorio:

   ```bash
   git clone https://github.com/tu-usuario/nombre-del-repositorio.git
   cd nombre-del-repositorio
