## Hola, soy Samuel 👋

Técnico de sistemas en Málaga. Administro **Active Directory, Windows Server y Microsoft 365 on-premise**, y automatizo con **PowerShell** e IA lo que antes se hacía a mano.

Aquí publico las herramientas que uso y lo que pruebo en mi laboratorio de casa. Todo está explicado para que lo pueda usar otro técnico.

### 🔧 En qué trabajo

- **Sistemas:** Active Directory, GPO, Windows Server, Microsoft 365, VMware ESXi, Hyper-V
- **Copias:** Veeam, Kopia, estrategia 3-2-1 con prueba de restauración
- **Automatización:** PowerShell, Python, tareas programadas, avisos por Telegram o Teams
- **Seguridad:** hardening de Windows y M365, certificados, acceso con mTLS. Bootcamp Red Team y certificado de ciberseguridad de Google
- **Laboratorio:** Hyper-V, Debian, Docker, NAS QNAP, Caddy, Tailscale

![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=flat&logo=powershell&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows%20Server-0078D4?style=flat&logo=windows&logoColor=white)
![Microsoft 365](https://img.shields.io/badge/Microsoft%20365-D83B01?style=flat&logo=microsoftoffice&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Debian](https://img.shields.io/badge/Debian-A81D33?style=flat&logo=debian&logoColor=white)

### 🩺 Kit del técnico de sistemas

Herramientas de PowerShell **de solo lectura** para revisar un equipo Windows en minutos: no cambian nada, generan informe HTML y JSON, y se prueban solas en cada cambio (CI con PowerShell 5.1 y 7). Las ejecuto en mis propios equipos antes de publicarlas.

| Herramienta | Qué revisa | Pruebas |
|---|---|---|
| [sysadmin-health-check](https://github.com/samuelmartindelgado/sysadmin-health-check) | **Todo el kit en un comando** e informe único con semáforo | [![CI](https://github.com/samuelmartindelgado/sysadmin-health-check/actions/workflows/ci.yml/badge.svg)](https://github.com/samuelmartindelgado/sysadmin-health-check/actions) |
| [windows-hardening-audit](https://github.com/samuelmartindelgado/windows-hardening-audit) | 23 comprobaciones de seguridad: SMBv1, LLMNR, NTLM, RDP, LAPS, BitLocker... | [![CI](https://github.com/samuelmartindelgado/windows-hardening-audit/actions/workflows/ci.yml/badge.svg)](https://github.com/samuelmartindelgado/windows-hardening-audit/actions) |
| [patch-status-report](https://github.com/samuelmartindelgado/patch-status-report) | Último parche, actualizaciones pendientes o fallidas, reinicio pendiente | [![CI](https://github.com/samuelmartindelgado/patch-status-report/actions/workflows/ci.yml/badge.svg)](https://github.com/samuelmartindelgado/patch-status-report/actions) |
| [pc-inventory](https://github.com/samuelmartindelgado/pc-inventory) | Inventario del equipo a CSV para toda la oficina: serie, RAM, discos, TPM, licencia, software | [![CI](https://github.com/samuelmartindelgado/pc-inventory/actions/workflows/ci.yml/badge.svg)](https://github.com/samuelmartindelgado/pc-inventory/actions) |
| [writable-path-audit](https://github.com/samuelmartindelgado/writable-path-audit) | Permisos mal puestos que dejarían a un usuario normal hacerse administrador | [![CI](https://github.com/samuelmartindelgado/writable-path-audit/actions/workflows/ci.yml/badge.svg)](https://github.com/samuelmartindelgado/writable-path-audit/actions) |
| [autostart-inventory](https://github.com/samuelmartindelgado/autostart-inventory) | Todo lo que arranca solo, con su firma digital y marcas de lo sospechoso | [![CI](https://github.com/samuelmartindelgado/autostart-inventory/actions/workflows/ci.yml/badge.svg)](https://github.com/samuelmartindelgado/autostart-inventory/actions) |
| [stale-local-accounts](https://github.com/samuelmartindelgado/stale-local-accounts) | Cuentas locales olvidadas, Administrador o Invitado activos, admins de más | [![CI](https://github.com/samuelmartindelgado/stale-local-accounts/actions/workflows/ci.yml/badge.svg)](https://github.com/samuelmartindelgado/stale-local-accounts/actions) |
| [cert-expiry-scanner](https://github.com/samuelmartindelgado/cert-expiry-scanner) | Certificados del equipo a punto de caducar y qué servicio fallará | [![CI](https://github.com/samuelmartindelgado/cert-expiry-scanner/actions/workflows/ci.yml/badge.svg)](https://github.com/samuelmartindelgado/cert-expiry-scanner/actions) |
| [time-drift-check](https://github.com/samuelmartindelgado/time-drift-check) | Hora mal sincronizada antes de que falle Kerberos o un certificado | [![CI](https://github.com/samuelmartindelgado/time-drift-check/actions/workflows/ci.yml/badge.svg)](https://github.com/samuelmartindelgado/time-drift-check/actions) |
| [event-log-size-check](https://github.com/samuelmartindelgado/event-log-size-check) | Registros de eventos que se sobrescriben en horas y no dejan rastro | [![CI](https://github.com/samuelmartindelgado/event-log-size-check/actions/workflows/ci.yml/badge.svg)](https://github.com/samuelmartindelgado/event-log-size-check/actions) |

### 🏠 Laboratorio

| Proyecto | De qué va |
|---|---|
| [homelab](https://github.com/samuelmartindelgado/homelab) | Mi laboratorio gestionado como el de una empresa: copias que se comprueban solas, monitor que solo avisa cuando algo cambia, baúl de secretos cifrado y encendido remoto |

Próximamente: herramientas de PowerShell para Active Directory, probadas en un laboratorio de dominio propio.

### 🧭 Cómo trabajo

- Primero en el laboratorio, luego en producción, y siempre con copia previa.
- Las herramientas de revisión son de solo lectura; lo que cambia algo tiene modo de prueba (`-WhatIf`).
- Las contraseñas nunca van dentro de un script.

### 📫 Contacto

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Samuel%20Martin%20Delgado-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/antonio-samuel-martin-delgado/)
