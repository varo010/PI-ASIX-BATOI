# Proyecto Red Empresarial – Grupo 3

## Descripción

Proyecto del ciclo formativo de grado superior de Administración de Sistemas Informáticos en Red (ASIX), desarrollado por el Grupo 3. Consiste en diseñar, montar y configurar la red interna de una empresa simulada utilizando los equipos físicos del taller, aplicando segmentación del tráfico, medidas de seguridad y almacenamiento centralizado.

## Objetivos

1. Segmentar la red mediante VLANs por departamento, aislando el tráfico entre las distintas áreas de la empresa.
2. Implementar medidas de seguridad mediante un firewall y listas de control de acceso (ACLs) que regulen la comunicación entre segmentos.
3. Configurar un NAS como almacenamiento centralizado, accesible desde los equipos cliente de la red.

## Instalación

Para que un equipo cliente Linux (Debian/Ubuntu) pueda montar los recursos compartidos del NAS mediante NFS, es necesario instalar el paquete cliente:

```bash
sudo apt install nfs-common
```

## Documentación de referencia

- [Documentación oficial de TrueNAS](https://www.truenas.com/docs/)

## Estado del proyecto

### Tareas realizadas

- [x] Formación del grupo y reparto de roles.
- [x] Identificación del hardware del taller disponible para el proyecto.

### Tareas pendientes

- [ ] Diseño del esquema lógico de red y del plan de direccionamiento IP.
- [ ] Configuración de VLANs, ACLs y del NAS.

## Autor

**Álvaro Pérez Morilla** (Grupo 3) – Ciclo Formativo de Grado Superior ASIX
