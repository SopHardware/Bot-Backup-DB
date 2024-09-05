# Arquitectura del Proyecto

La arquitectura del proyecto será de capas, con las siguientes capas:

- **Capa de acceso a datos (DAL):** se encargará de interactuar con la base de datos y realizar las operaciones de respaldo.
- **Capa de negocio (BLL):** se encargará de procesar la información y realizar las operaciones de comprimir y encriptar los archivos de respaldo.
- **Capa de presentación (PL):** se encargará de interactuar con el usuario y mostrar los resultados del proceso de respaldo.

## Estructura de las Carpetas y sus Clases

### **BackupDB:** carpeta raíz del proyecto

- **BackupDB.DAL:** carpeta de la capa de acceso a datos
- **BackupDB.BLL:** carpeta de la capa de negocio
- **BackupDB.PL:** carpeta de la capa de presentación
- **BackupDB.Models:** carpeta de modelos de datos
- **BackupDB.Utils:** carpeta de utilidades

### **BackupDB.DAL:**

- `Database.cs:` clase que representa una base de datos
- `Backup.cs:` clase que realiza el respaldo de una base de datos
- `DatabaseRepository.cs:` clase que interactúa con la base de datos y realiza las operaciones de respaldo

### **BackupDB.BLL:**

- `BackupProcessor.cs:` clase que procesa la información y realiza las operaciones de comprimir y encriptar los archivos de respaldo
- `ReportGenerator.cs:` clase que genera un reporte sobre el estatus de cada respaldo realizado

### **BackupDB.PL:**

- `BackupForm.cs:` clase que interactúa con el usuario y muestra los resultados del proceso de respaldo

### **BackupDB.Models:**

- `DatabaseModel.cs:` clase que representa un modelo de datos de una base de datos
- `BackupModel.cs:` clase que representa un modelo de datos de un respaldo

### **BackupDB.Utils:**

- `Compression.cs:` clase que comprime los archivos de respaldo
- `Encryption.cs:` clase que encripta los archivos de respaldo
