# DropDownsAnidadosMvc

Proyecto ASP.NET MVC con **dropdowns anidados** (cascada) para gestión de productos. La selección de **Categoría** filtra **Sucursales** y **Productos** vía AJAX.

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

Controllers/
├── HomeController.cs          # Página principal
├── ProductosController.cs     # CRUD Productos + AJAX endpoints
└── MigracionesController.cs   

## Models
Models/
├── Categoria.cs               # Modelo Categoría
├── Sucursal.cs                # Modelo Sucursal  
├── Producto.cs                # Modelo Producto principal
└── DropDownVM.cs              # ViewModel para dropdowns
## Views
Views/
├── Home/
│   └── Index.cshtml
├── Productos/
│   ├── Create.cshtml         # Crear con dropdowns anidados
│   ├── Delete.cshtml
│   ├── Details.cshtml
│   ├── Edit.cshtml
│   └── Index.cshtml          # Listado productos
└── Shared/
    └── _Layout.cshtml




## Tecnologías

| Backend                   | Frontend          | Base de datos |
| ------------------------- | ----------------- | ------------- |
| ASP.NET MVC Core          | Bootstrap, jQuery | SQL Server    |
| C#, Entity Framework Core | JavaScript/AJAX   | LocalDB       |
