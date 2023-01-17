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

### Seahaven
Servidor Debian Bullseye desde el que lanzaremos los playbooks.
Sobre este nodo ejecutaremos un script de pre-aprovisionamiento para evitar
incompatibilidades de Vagrant con Virtualbox y he decidido atacar a bajo nivel
desde un shell script.

Hará de bastión simulando ser una plataforma cloud genérica.

## Dependencias
* Virtualbox o KVM/Qemu
* Vagrant >= 2.3.4


## Apéndices
