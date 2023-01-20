# Observability

Repositorio para formación en observability sobre sistemas GNU/Linux.

## Tecnologías que usaremos
* Rsyslog
* logrotate
* Ansible

## Componentes
### Máquinas virtuales
* **Truman:** Red Hat Enterprise Linux observada
* **Christof:** Colector de información
* **Seahaven:** Bastión Ansible

### Christof
Nodo RHEL 8 que hará las veces de colector de métricas varias:
* Logs de sistema
* Logs de aplicación
* APM
* Rendimiento de los sistemas

### Seahaven
Servidor Debian Bullseye desde el que lanzaremos los playbooks.
El objetivo con **seahaven** es simular un entorno independiente a la plataforma
final sobre la que ejecutaremos nuestros playbooks de aprovisionamiento. La 
*Definition of Ready* vendrá determinada por la encapsulación completa y portable
del directorio *platform* y su contenido al completo; es decir, dentro de dicho
directorio deberíamos poder gestionar un repositorio de git independiente al
resto de IaC.

### Truman
Nodo RHEL 8 que enviará todo tipo de métricas a Christof.
#### Software que incluye
- [ ] Filebeat
- [ ] Sysstat
- [ ] Apache

Hará de bastión simulando ser una plataforma cloud genérica.

## Dependencias
* Virtualbox o KVM/Qemu
* Vagrant >= 2.3.4


## Apéndices
### Dotfiles
* [dotfiles/vimrc](dotfiles/vimrc)
