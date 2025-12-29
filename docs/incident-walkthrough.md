# Incident Walkthrough — IAM Lab (Active Directory)

## 🇬🇧 English version

This document provides a step-by-step walkthrough of the IAM lab, showing the environment state before the incident and the actions performed during the investigation.

---

## Identity and Domain Preparation

A dedicated Organizational Unit and a standard domain user were created to simulate a controlled IAM environment.

![User and OU creation](images/02_creacion_usuario_ou.png)

---

## Client Joined to the Domain

The client machine was successfully joined to the Active Directory domain.

![Client joined to domain](images/03_cliente_en_dominio.png)

---

## Normal Authentication (Baseline)

Before the incident, the domain user was able to authenticate successfully, establishing normal behavior.

![Domain login screen](images/01_Inicio_de_sesion_dominio.png)

![Successful domain login](images/04_login_correcto.png)

---

## Incident Trigger

After the baseline was established, failed authentication attempts were generated against the domain user.

The detection, analysis, containment, and validation phases of the incident are documented in the main README.md file.

---

# Guía del incidente — Laboratorio IAM (Active Directory)

## 🇪🇸 Versión en español

Este documento describe paso a paso el desarrollo del laboratorio IAM, mostrando el estado normal del entorno antes del incidente y las acciones realizadas durante la investigación.

---

## Preparación de identidades y dominio

Se creó una Unidad Organizativa dedicada y un usuario de dominio estándar para simular un entorno IAM controlado.

![Creación de usuario y OU](images/02_Creacion_usuario_OU.png)

---

## Cliente unido al dominio

El equipo cliente se unió correctamente al dominio de Active Directory.

![Cliente unido al dominio](images/03_Cliente_en_dominio.png)

---

## Autenticación normal (estado base)

Antes del incidente, el usuario de dominio podía iniciar sesión correctamente, estableciendo el comportamiento normal del sistema.

![Pantalla de inicio de sesión en dominio](images/01_Inicio_de_sesion_dominio.png)

![Inicio de sesión correcto](images/04_Acceso_cliente_a_dominio.png)

---

## Inicio del incidente

Una vez establecido el estado base, se generaron intentos fallidos de autenticación contra el usuario de dominio.

Las fases de detección, análisis, contención y validación del incidente se documentan en el archivo principal README.md.
