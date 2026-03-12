# DropDownsAnidadosMvc

Proyecto ASP.NET MVC con **dropdowns anidados** 

## Características

- Dropdowns en cascada: Categoría → Sucursal → Producto.
- CRUD completo para Productos (Create, Read, Update, Delete).
- Migraciones Entity Framework incluidas.
- Diseño responsive con Bootstrap.

## Requisitos

- Visual Studio 2022+ con ASP.NET MVC.
- .NET (ver tu target framework).
- SQL Server LocalDB.
- Entity Framework Core Tools.

## Instalación

1. **Clona el repo**:
   ```bash
   git clone https://github.com/sCastellan0/DropDownsAnidadosMvc.git
   cd DropDownsAnidadosMvc
2. **Abre DropDownsAnidadosMvc.sln en Visual Studio.**
3. **Configura conexión en appsettings.json.**
   "ConnectionStrings": {
  "DefaultConnection": "Server=(localdb)\\mssqllocaldb;Database=DropDownsDB;Trusted_Connection=true;MultipleActiveResultSets=true"
}
4. **Restaura paquetes: Right-click solution → Restore NuGet Packages.**
5. **Ejecuta migraciones (Package Manager Console)**
   Add-Migration InitialCreate
   Update-Database

# Estructura del Proyecto

<img width="298" height="257" alt="image" src="https://github.com/user-attachments/assets/ee682f4c-7290-4a62-a5c5-80650a617056" />





## Tecnologías

| Backend                   | Frontend          | Base de datos |
| ------------------------- | ----------------- | ------------- |
| ASP.NET MVC Core          | Bootstrap, jQuery | SQL Server    |
| C#, Entity Framework Core | JavaScript/AJAX   | LocalDB       |
