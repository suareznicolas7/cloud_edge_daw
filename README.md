# # Tarea (a+b) · Cloud: niveles y funciones (DAW 1º)

## 🅰️ Tarea A — Niveles de cloud (IaaS/PaaS/SaaS)
Crea una tabla con 10 servicios reales. Incluye enlace oficial y justifica responsabilidades.

# Niveles de Cloud: IaaS / PaaS / SaaS

| Servicio | Proveedor | Nivel | Enlace oficial | ¿Qué gestiona el proveedor? | ¿Qué gestiona el equipo/usuario? |
|---------|----------|-------|----------------|-----------------------------|----------------------------------|
| IBM Cloud Virtual Servers | IBM | IaaS | https://www.ibm.com/cloud/virtual-servers | Centro de datos, hardware, virtualización y red. | Sistema operativo, aplicaciones, parches y datos. |
| Oracle Compute VM | Oracle Cloud | IaaS | https://www.oracle.com/cloud/compute/ | Infraestructura física, red y virtualización. | Sistema operativo, software y seguridad. |
| Alibaba Cloud ECS | Alibaba Cloud | IaaS | https://www.alibabacloud.com/product/ecs | Servidores físicos, red y almacenamiento. | Sistema operativo, aplicaciones y datos. |
| Red Hat OpenShift | Red Hat | PaaS | https://www.redhat.com/openshift | Plataforma de contenedores, SO base, escalado. | Código de aplicaciones y datos. |
| Firebase | Google | PaaS | https://firebase.google.com/ | Backend, base de datos, autenticación y escalado. | Lógica de la aplicación y frontend. |
| Platform.sh | Platform.sh | PaaS | https://platform.sh/ | Infraestructura, runtime y despliegue. | Código y configuración de la app. |
| Zoom | Zoom Video Communications | SaaS | https://zoom.us/ | Aplicación, infraestructura y mantenimiento. | Uso de la herramienta y gestión de usuarios. |
| Trello | Atlassian | SaaS | https://trello.com/ | Software, servidores y actualizaciones. | Tableros, tareas y usuarios. |
| Shopify | Shopify | SaaS | https://www.shopify.com/ | Plataforma e infraestructura de comercio electrónico. | Productos, pedidos y contenido. |
| GitHub | Microsoft | SaaS | https://github.com/ | Aplicación, servidores y seguridad. | Repositorios, código y permisos. |

## 🅱️ Tarea B — Funciones principales de cloud (arquitectura)
Incluye un diagrama (ASCII/Mermaid/imagen) y una explicación breve.

### Diagrama

          +----------------+
          |   Usuarios     |
          +--------+-------+
                   |
                   v
          +----------------+
          |  Frontend /    |
          |   Cliente      |
          +--------+-------+
                   |
                   v
          +----------------+
          | Balanceador de |
          |     carga      |
          +--------+-------+
                   |
       +-----------+-----------+
       |                       |
       v                       v
+--------------+        +--------------+
| Aplicaciones |        | Monitorización|
| / Servicios  |        +--------------+
+------+-------+
       |
       +-----------------+
       |                 |
       v                 v
+--------------+    +--------------+
| Base de datos|    | Almacenamiento|
+--------------+    +--------------+
       |
       v
+--------------+
| Seguridad y  |
| control de   |
| acceso       |
+--------------+

### Explicación (8–12 líneas)
(Describe el flujo front → API → BBDD/storage y dónde entra la cloud)



### Mapeo de funciones cloud a componentes (mínimo 3)
- Procesamiento → …
- Ejecución → …
- Almacenamiento → …
- Intercambio → … (opcional si ya tienes 3)

## 📚 Fuentes (enlaces oficiales)
(Enlaces oficiales usados en la tabla A y en la B)
