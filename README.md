# CRM · Customer Relationship Management

Aplicación de escritorio para gestionar la relación con los clientes de una empresa: comerciales, empresas cliente, agenda de acciones (llamadas, emails y visitas) y estadísticas de ventas.

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Swing](https://img.shields.io/badge/Swing-5382A1?style=flat-square&logo=openjdk&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat-square&logo=apachemaven&logoColor=white)

> [!NOTE]
> Proyecto en equipo del FP DAM. Cada integrante trabajó en su propia rama.

## Demo

- 🎬 [Vídeo explicativo](https://www.youtube.com/watch?v=w1MzpbHB-tY)
- 📘 [Manual de usuario (PDF)](Manual%20Usuario%20CRM.pdf)

## Funcionalidades

| Módulo | Qué hace |
|---|---|
| Login | Acceso para gestores y comerciales |
| Comerciales | Alta, edición y consulta del equipo comercial |
| Empresas | Fichas de las empresas cliente |
| Agenda | Registro de llamadas, emails y visitas a cada cliente |
| Estadísticas | Gráficas y ranking de comerciales |
| Exportación | Datos a Excel |

## Tecnologías

| Capa | Tecnología |
|---|---|
| Lenguaje | Java |
| Interfaz | Swing (NetBeans), JCalendar y JDatePicker |
| Base de datos | MySQL (JDBC) |
| Gráficas | JFreeChart |
| Excel | Apache POI |
| Logs | Log4j |

## Estructura

```
├── CRM/                        Proyecto Maven
│   └── src/main/java/com/mycompany/crm/
│       ├── gui/                Pantallas (login, menú, agenda, estadísticas…)
│       └── …                   Modelo, acceso a datos (DAO) y validaciones
├── CRM_BBDD.sql                Script para crear la base de datos
├── Data/                       Datos de ejemplo (clientes y empleados)
├── diagramaRelacionalCRM.JPG   Diagrama de la base de datos
└── Manual Usuario CRM.pdf      Manual de usuario
```

## Cómo ejecutarlo

1. Crea la base de datos en MySQL con `CRM_BBDD.sql` (se conecta a `localhost:3306/crm`).
2. Abre la carpeta `CRM/` en NetBeans o IntelliJ como proyecto Maven.
3. Ejecuta la clase principal.

## Diagrama de la base de datos

![Diagrama relacional](diagramaRelacionalCRM.JPG)
