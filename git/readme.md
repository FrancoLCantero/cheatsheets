[Volver a sección principal](https://github.com/FrancoLCantero/cheatsheets/tree/main)

# **Apuntes de Git**

## **1. Introducción a Git**
Git es un sistema de control de versiones distribuido, que permite rastrear cambios en archivos y coordinar el trabajo en esos archivos entre múltiples personas.

### **1.1. Instalación de Git**
Puedes instalar Git en tu sistema operativo desde [git-scm.com](https://git-scm.com/). Una vez instalado, verifica la instalación con:

```bash
git --version
```

## **2. Configuración Inicial**

### **2.1. Configuración Global de Usuario**
Configura tu nombre de usuario y correo electrónico globales para que Git los use por defecto:

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tuemail@ejemplo.com"
```

### **2.2. Ver Configuración**
Para ver tu configuración global:

```bash
git config --list
```

O para ver un ajuste específico:

```bash
git config user.name
git config user.email
```

## **3. Trabajando con Repositorios**

### **3.1. Iniciar un Nuevo Repositorio**
Para iniciar un nuevo repositorio Git en un directorio existente:

```bash
cd ruta/a/tu/proyecto
git init
```

Esto crea un subdirectorio oculto llamado `.git` que contiene todos los archivos necesarios para el repositorio.

### **3.2. Clonar un Repositorio**
Para clonar un repositorio existente:

```bash
git clone url-del-repositorio
```

Esto creará un directorio con el nombre del repositorio y descargará su contenido.

## **4. Realizando Cambios**

### **4.1. Ver el Estado del Repositorio**
Para ver el estado de tus archivos y cambios:

```bash
git status
```

### **4.2. Añadir Archivos al Área de Preparación (Stage)**
Antes de confirmar (commit) los cambios, se deben añadir al área de preparación:

```bash
git add nombre_del_archivo
```

Para añadir todos los archivos:

```bash
git add .
```

### **4.3. Hacer un Commit**
Para guardar los cambios en el historial del repositorio:

```bash
git commit -m "Mensaje descriptivo sobre el cambio"
```

### **4.4. Ver el Historial de Commits**
Para ver el historial de commits:

```bash
git log
```

Para un historial más compacto:

```bash
git log --oneline
```

## **5. Trabajando con Repositorios Remotos**

### **5.1. Añadir un Repositorio Remoto**
Para añadir un repositorio remoto:

```bash
git remote add origin url-del-repositorio-remoto
```

### **5.2. Ver Repositorios Remotos**
Para listar los repositorios remotos configurados:

```bash
git remote -v
```

### **5.3. Hacer Push**
Para enviar tus commits locales al repositorio remoto:

```bash
git push origin nombre_de_la_rama
```

Si es la primera vez que empujas una rama, puede que necesites usar:

```bash
git push -u origin nombre_de_la_rama
```

### **5.4. Hacer Pull**
Para actualizar tu repositorio local con los cambios del remoto:

```bash
git pull origin nombre_de_la_rama
```

Esto combinará los cambios del remoto con tu rama actual.

## **6. Ramas (Branches)**

### **6.1. Crear una Nueva Rama**
Para crear y cambiar a una nueva rama:

```bash
git checkout -b nombre_de_la_rama
```

### **6.2. Cambiar de Rama**
Para cambiar a una rama existente:

```bash
git checkout nombre_de_la_rama
```

### **6.3. Ver Ramas Existentes**
Para listar todas las ramas:

```bash
git branch
```

### **6.4. Fusionar Ramas**
Para fusionar cambios de una rama a otra:

1. Cambia a la rama en la que quieres fusionar los cambios (por ejemplo, `main`):

```bash
git checkout main
```

2. Fusión:

```bash
git merge nombre_de_la_rama
```

## **7. Deshacer Cambios**

### **7.1. Revertir un Archivo al Último Commit**
Para deshacer cambios en un archivo que no ha sido añadido al stage:

```bash
git checkout -- nombre_del_archivo
```

### **7.2. Restablecer el Stage**
Para quitar archivos del área de preparación:

```bash
git reset nombre_del_archivo
```

### **7.3. Revertir un Commit**
Para revertir un commit específico:

```bash
git revert id_del_commit
```

### **7.4. Restablecer el Repositorio**
Para restablecer el estado del repositorio a un commit anterior:

```bash
git reset --hard id_del_commit
```

## **8. Otros Comandos Útiles**

### **8.1. Ignorar Archivos**
Para ignorar archivos o directorios específicos, añade sus patrones en un archivo `.gitignore`.

### **8.2. Guardar Trabajo Incompleto (Stash)**
Si necesitas cambiar de rama pero quieres guardar tu trabajo actual:

```bash
git stash
```

Para aplicar el último stash:

```bash
git stash apply
```

Para listar los stashes guardados:

```bash
git stash list
```

[Volver a sección principal](https://github.com/FrancoLCantero/cheatsheets/tree/main)

---
Last Edited on: 12/12/2024
