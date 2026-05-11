# NUBES-INTERMODULAR
# ☁️ Red BridgeWay English: Infraestructura en la Nube (AWS)

¡Bienvenido al motor digital de mi academia! En esta sección del proyecto de 1º de SMR, documento cómo he trasladado la gestión y el almacenamiento de **Red BridgeWay English** a la nube de Amazon Web Services (AWS).

## 🚀 El Concepto: "Academia Non-Stop"
El objetivo de este diseño es que la academia nunca se detenga. He eliminado la dependencia de servidores físicos y pendrives para evitar:
1. **Pérdida de datos** por fallos de hardware.
2. **Infecciones por malware** a través de dispositivos USB.
3. **Falta de acceso** de los profesores a sus materiales desde fuera del centro.

---

## 🏗️ Arquitectura de Red (VPC)
He diseñado una **VPC (Virtual Private Cloud)** a medida, segmentando la red para que sea segura y eficiente:
- **Red Privada:** Los datos de los alumnos están protegidos.
- **Internet Gateway:** Permite la salida controlada a internet para actualizaciones y sincronización.
- **Tablas de Enrutamiento:** Gestionan el tráfico para que la administración y las aulas no se interfieran.

> [!TIP]
> Puedes ver el mapa lógico detallado en el archivo `nubes-red-intermodular.png` dentro de esta carpeta.

---

## 🛠️ Servicios AWS Implementados

| Servicio | Función en la Academia | Beneficio Real |
| :--- | :--- | :--- |
| **Amazon S3** | Repositorio de Listenings y PDFs | Acceso instantáneo y seguro para los profes. |
| **Amazon RDS** | Base de Datos de Alumnos | Copias de seguridad automáticas de matrículas y notas. |
| **Amazon EC2** | Servidores de Gestión | Potencia de cálculo sin necesidad de hardware físico caro. |
| **AWS IAM** | Control de Accesos | Cada usuario (profe/admin) solo entra a lo que necesita. |

---

## 📊 Documentación Técnica
He preparado un manual detallado donde explico paso a paso la configuración y la "humanización" de esta tecnología:

👉 **[Descargar Documentación Nubes (PDF)](./DOCUMENTACIÓN%20NUBES%20INTERMODULAR.pdf)**

---

## 💡 Cultura IT
Este proyecto no trata solo de conectar cables, sino de trabajar con metodología:
- **Escalabilidad:** Si abrimos más aulas, la nube crece con nosotros.
- **Seguridad:** Aplicamos el principio de menor privilegio (IAM).
- **Disponibilidad:** Si un PC de la academia falla, el trabajo sigue en la nube.

---
*Configurado por **David Castro** - Proyecto Intermodular 1º SMR*
