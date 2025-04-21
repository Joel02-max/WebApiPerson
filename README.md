# Proyecto .NET con Conexión a Base de Datos SQL Server

Este repositorio documenta el proceso completo para la creación de una aplicación en Visual Studio utilizando .NET, C# y SQL Server. 
El enfoque principal es la creación de una API RESTful que se conecta a una base de datos y expone operaciones CRUD para el manejo de entidades como 'Persona'.

---

# 📌 Desarrollo

- Introducción a entornos gráficos y Microsoft .NET
- Instalación de herramientas necesarias
- Creación de una base de datos en SQL Server
- Desarrollo de una API en .NET
- Conexión a base de datos con Entity Framework
- Pruebas de la API

---

## 🧠 Conceptos Teóricos

### .NET

Plataforma de desarrollo 'open source' para crear aplicaciones web, móviles, de escritorio y más. Componentes clave:

- **Librerías**
- **Lenguajes**: C#
- **Versiones clave**:
  - .NET Framework
  - .NET Core


### SQL Server Management Studio (SSMS)

Entorno gráfico integrado para gestionar bases de datos SQL Server local o en Azure.

### API (Application Programming Interface)

Una interfaz que permite que diferentes aplicaciones se comuniquen entre sí. En este caso, construiremos una API , que se basa en:

- Interfaz uniforme
- Métodos HTTP (CRUD)
  - `GET` - Obtener
  - `POST` - Crear
  - `PUT` - Editar
  - `DELETE` - Eliminar

---

## 🧰 Instalación de Herramientas

### 1. Visual Studio Community

Instalar desde: https://visualstudio.microsoft.com/es/vs/community/

Seleccionar carga de trabajo **ASP.NET y desarrollo web**.

### 2. .NET SDK

Instalación automática con Visual Studio.

### 3. SQL Server y SSMS

- Descargar SSMS (SQL Server Management Studio)
  (https://learn.microsoft.com/en-us/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16)
- Instalar SQL Server Express o Developer Edition
- Crear instancia local

---

## 🛠️ Desarrollo del Proyecto

### 1. Crear Base de Datos

Desde SSMS:

- Base de datos: donde mediante visual studio crearemos una tabla 'Personas'

### 2. Crear Proyecto API en Visual Studio

1. Nuevo proyecto → ASP.NET Core Web API
2. Elegir .NET 
3. Crearmos las# carpetas:
   - Models
   - Controllers

### 3. Modelo Persona
Ejemplo  csharp
````
public class Persona
{
    public int Id { get; set; }
    public string Nombre { get; set; }
    public string Apellido { get; set; }
}
````
---
### Creación de la API RESTful

- **Métodos CRUD**:
  - **Crear
  - **Recuperar
  - **Update 
  - **Delete 

### Instalación de Paquetes

- Utiliza NuGet para instalar los paquetes necesarios para la conexión a la base de datos.

### Comando para Actualizar la Base de Datos

```bash
PM> Update-Database
```

## Pruebas de la API

- Prueba la API utilizando url.
- Realiza peticiones GET, POST, PUT y DELETE para verificar la funcionalidad.

