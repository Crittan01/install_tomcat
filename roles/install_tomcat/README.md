# Role install_tomcat

Este rol se encarga de instalar y configurar Apache Tomcat en servidores RHEL/CentOS y Ubuntu. Soporta la generación de certificados SSL autofirmados y permite el despliegue de una aplicación de prueba.

## Requirements

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

## Role Variables

- `tomcat_port`: Puerto HTTP en el que se ejecuta Tomcat.
- `tomcat_ssl_enabled`: Habilitar o deshabilitar HTTPS.
- `tomcat_admin_user`: Usuario administrador de Tomcat.

## Funcionalidades:

- Instalación de Tomcat.
- Configuración de SSL con un certificado autofirmado.
- Apertura de puertos en el firewall.
- Despliegue de una aplicación de ejemplo.

## Dependencies

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

## License

BSD

## Author Information

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
