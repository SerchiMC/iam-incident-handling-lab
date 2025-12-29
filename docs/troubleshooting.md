# Troubleshooting — VirtualBox

## 🇬🇧 English version

## Issue
VirtualBox failed to start virtual machines with the following error:

VERR_NEM_VM_CREATE_FAILED

## Root Cause
A conflict between VirtualBox and Windows native virtualization features was identified.  
Specifically, the following components were enabled on the host system:

- Hyper-V
- Virtual Machine Platform
- Windows Hypervisor Platform
- Virtualization-Based Security (VBS)
- Core Isolation / Memory Integrity

These features prevent VirtualBox from accessing hardware virtualization directly.

## Resolution
The issue was resolved by disabling the conflicting Windows features:

- Hyper-V
- Virtual Machine Platform
- Windows Hypervisor Platform
- Core Isolation (Memory Integrity)

After applying the changes, the system was rebooted.

## Outcome
Once the host system restarted, VirtualBox was able to start virtual machines normally and the lab environment was deployed successfully.

---

# Resolución de problemas — VirtualBox

## 🇪🇸 Versión en español

## Problema
VirtualBox no podía iniciar las máquinas virtuales y mostraba el siguiente error:

VERR_NEM_VM_CREATE_FAILED

## Causa raíz
Se detectó un conflicto entre VirtualBox y las funcionalidades de virtualización nativas de Windows.  
En concreto, estaban activados los siguientes componentes en el sistema anfitrión:

- Hyper-V
- Plataforma de máquina virtual
- Plataforma del hipervisor de Windows
- Seguridad basada en virtualización (VBS)
- Aislamiento del núcleo / Integridad de memoria

Estas funcionalidades impiden que VirtualBox acceda directamente a la virtualización por hardware.

## Resolución
El problema se solucionó desactivando las funcionalidades de Windows que entraban en conflicto:

- Hyper-V
- Plataforma de máquina virtual
- Plataforma del hipervisor de Windows
- Aislamiento del núcleo (Integridad de memoria)

Tras aplicar los cambios, se reinició el sistema.

## Resultado
Después del reinicio, VirtualBox pudo iniciar las máquinas virtuales con normalidad y el entorno del laboratorio se desplegó correctamente.
