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

El flujo comienza en el **front-end**, donde el usuario realiza una acción que envía una solicitud a la **API**. Esta API procesa la solicitud, ejecuta la lógica de negocio y, si es necesario, interactúa con la **base de datos (BBDD)** o el **almacenamiento (storage)** para recuperar o almacenar información. La **cloud** entra en juego cuando la base de datos o el almacenamiento están ubicados en la nube, ofreciendo escalabilidad, alta disponibilidad y gestión eficiente de recursos. Después de procesar la solicitud, la **API** responde al **front-end** con los datos o resultados solicitados. Finalmente, el **front-end** actualiza la interfaz de usuario con la información recibida, completando el ciclo de interacción.

### Mapeo de funciones cloud a componentes (mínimo 3)

* **Procesamiento →** Servicios gestionados de la cloud (por ejemplo, funciones serverless) que ejecutan la lógica de negocio y procesan las peticiones de la API.
* **Ejecución →** Máquinas virtuales o contenedores en la nube donde se despliega el back-end y la API.
* **Almacenamiento →** Bases de datos en la nube y servicios de storage para guardar información persistente (datos, archivos, copias de seguridad).
* **Intercambio →** Servicios de red y APIs cloud que permiten la comunicación segura entre front-end, back-end y otros servicios.

## 📚 Fuentes (enlaces oficiales)
(Enlaces oficiales usados en la tabla A y en la B)

Claro, aquí tienes solo los enlaces de cada apartado:

1. **IBM Cloud Virtual Servers**: [https://www.ibm.com/cloud/virtual-servers](https://www.ibm.com/cloud/virtual-servers)
2. **Oracle Compute VM**: [https://www.oracle.com/cloud/compute/](https://www.oracle.com/cloud/compute/)
3. **Alibaba Cloud ECS**: [https://www.alibabacloud.com/product/ecs](https://www.alibabacloud.com/product/ecs)
4. **Red Hat OpenShift**: [https://www.redhat.com/openshift](https://www.redhat.com/openshift)
5. **Firebase**: [https://firebase.google.com/](https://firebase.google.com/)
6. **Platform.sh**: [https://platform.sh/](https://platform.sh/)
7. **Zoom**: [https://zoom.us/](https://zoom.us/)
8. **Trello**: [https://trello.com/](https://trello.com/)
9. **Shopify**: [https://www.shopify.com/](https://www.shopify.com/)
10. **GitHub**: [https://github.com/](https://github.com/)

