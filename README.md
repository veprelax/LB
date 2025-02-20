> Виконувала самостійно Слобожан Софія РПЗ-23А

  ### Лабораторна_ робота №1 

Topic: Introduction to the Virtual Machine Environment and Features of the Linux Operating System

Objective:

1.Familiarization with different types of hypervisors and virtualization in operating systems.

2.Overview of modern operating systems and their capabilities.

 _**Glossary of Terms**_

- Hypervisor – Software that creates and manages virtual machines.

- Virtualization – Technology that enables multiple operating systems to run on a single physical device.

- Type 1 Hypervisor – Runs directly on hardware without requiring an operating system.

- Type 2 Hypervisor – Runs on top of an operating system and utilizes its resources to create virtual machines.

- Virtual Machine (VM) – A software-based emulation of a computer that allows operating systems to run in an isolated environment.

- Guest OS – An operating system running inside a virtual machine.

- Host OS – The operating system running on physical hardware that manages the hypervisor.

- KVM (Kernel-based Virtual Machine) – A hypervisor built into the Linux kernel.

- VMware – A popular virtualization solution supporting both server and desktop environments.

- VirtualBox – A cross-platform Type 2 hypervisor developed by Oracle.

_Answers to Questions_

1. Define the term "hypervisor." What are its types?
A hypervisor is software that allows the creation and management of virtual machines. It distributes resources among guest operating systems and ensures their isolation.
There are two main types of hypervisors:

Type 1 Hypervisors – Run directly on hardware without requiring a host OS. Examples: Xen, Microsoft Hyper-V, VMware ESXi.

Type 2 Hypervisors – Installed on top of a host operating system. Examples: VirtualBox, VMware Workstation.
Main Components and Features of the Hyper-V Hypervisor
15 варіант

Hyper-V is a Type 1 hypervisor developed by Microsoft for running virtual machines on Windows-based systems.

_Main Components:_
Hyper-V Manager – A graphical tool for managing virtual machines.
Virtual Machine Monitor (VMM) – Manages the execution and resource allocation of virtual machines.
Hyper-V Virtual Switch – A virtual networking component that enables VM-to-VM and VM-to-external communication.
Integration Services – A set of drivers and utilities that improve VM performance and interaction with the host OS.
Storage Migration – Allows moving virtual disks between different storage locations without downtime.
Checkpoints (Snapshots) – Enable saving the state of a VM for quick restoration.
Dynamic Memory – Allocates RAM dynamically based on VM needs.
Live Migration – Enables moving VMs between physical hosts without interruption.
Key Features:
Supports Windows and Linux guest operating systems.
Provides resource isolation and secure virtualization.
Includes GPU virtualization for enhanced graphics performance.
Offers high availability and disaster recovery features.
Supports nested virtualization for running VMs inside VMs.
Compatible with Windows Admin Center for remote management.
_Хід роботи._
Подивіться ознайомчі відео та демонстраційні матеріали з наступних напрямків:
Linux - Кращі дистрибутиви 2023 https://youtu.be/PahmJBU9HKA?si=maxRf0nZlqs2hFGU 
ТОП 5 ПРИЧИН ЧОМУ АЙТІШНИКУ ВАРТО ПЕРЕЙТИ НА ЛІНУКС  
       Доступ: https://youtu.be/bP3_mZKezvM?si=sM3Mpc9JQ_0bY9Yd   
Як встановити Linux разом з Windows спосіб #1 Microsoft Store  
       Доступ: https://youtu.be/eEdGl6HvSdM?si=WDbwa71i034D2rQj  
Як встановити Linux разом з Windows спосіб #2 Dual Boot 
       Доступ: https://youtu.be/Hfky8TEyXss?si=ilduY167LS-vKl9y   
Як встановлювати програми на Linux. Linux українською #1 
       Доступ: https://youtu.be/M8XHJME6cxI?si=L0Koom59jTRnPXnU  
Як зробити панель завдань Linux як у Windows. Linux українською #2 
       Доступ: https://youtu.be/9szAz-A4gaM?si=LxaVueluI3tKRb1r  
Як встановити Ubuntu на VirtualBox https://youtu.be/ADOaHm1VZII?si=hG5kDRsajFn7se8d 
The Shell (Linux) https://drive.google.com/open?id=0B0PV0_SM0LoDSVNPWUVRdUxaN2s
Linux Desktop Environments: XFCE vs GNOME vs KDE 
Доступ: https://youtu.be/2JBGQfPR5xQ?si=euswD7IHrODd-6JH 
_Контрольні запитання_

1. Compare Type 1 and Type 2 hypervisors. What is the difference and their application areas?

Type 1 Hypervisors (bare-metal) run directly on the physical hardware without requiring a host OS. They provide better performance, security, and scalability, making them ideal for enterprise servers and cloud computing environments. Examples: VMware ESXi, Microsoft Hyper-V, Xen.
Type 2 Hypervisors (hosted) run on top of an existing operating system and use its resources to create virtual machines. They are more suitable for desktop virtualization, testing, and development. Examples: VirtualBox, VMware Workstation.
2. Explain the concept of "GNU GPL." What is its main idea?
The GNU General Public License (GPL) is a free software license that ensures users have the freedom to use, modify, and distribute software. Its main idea is to promote open-source development and prevent proprietary restrictions on software derived from GPL-licensed projects.

3. What is the essence of open-source software?
Open-source software (OSS) is software whose source code is freely available for anyone to inspect, modify, and distribute. It fosters collaboration, transparency, and innovation while allowing developers to customize the software to meet their needs.

4. What is a distribution (distro)?
A Linux distribution (distro) is a packaged version of the Linux operating system that includes the Linux kernel, system utilities, applications, and package management tools. Examples: Ubuntu, Fedora, Debian, Arch Linux.

5. What system administration tasks can be performed on Linux?

User and group management
File system and disk management
Network configuration and monitoring
Service and process management
Security configurations (firewall, SELinux, AppArmor)
System updates and package management
Backup and recovery procedures
Server deployment (web, database, DNS, etc.)
6. How are Android and Linux related?
Android is based on the Linux kernel, which manages hardware and system processes. However, Android differs from traditional Linux distributions as it uses its own runtime environment, libraries, and UI framework optimized for mobile devices.

7. What are the main features and applications of Embedded Linux?
Embedded Linux is a lightweight and customized version of Linux designed for embedded systems such as routers, IoT devices, smart TVs, and automotive systems.
Features:

Minimal resource usage
Custom kernel modifications
High stability and security
Real-time capabilities (with RT patches)
Applications:
Smart home devices (Raspberry Pi, OpenWRT)
Industrial automation
Automotive infotainment systems
Medical devices
8. How can you change the Linux boot type: text mode (runlevel 3) or graphical mode (runlevel 5)? What is the difference between CLI and GUI?
To change the boot mode in Linux:

Temporarily: At the boot menu (GRUB), press e, find the line with linux, and add 3 (text mode) or 5 (GUI mode) at the end.
Permanently: Modify the default target:
Text mode: sudo systemctl set-default multi-user.target
GUI mode: sudo systemctl set-default graphical.target
CLI (Command Line Interface) vs. GUI (Graphical User Interface):

CLI: Uses text-based commands; efficient for advanced users, scripting, and automation.
GUI: Provides a graphical environment with windows, icons, and menus; easier for beginners but may consume more system resources.
Оформлення звіту:
Титульний аркуш
Тема та мета роботи
Завдання попередньої підготовки
Основні позиції ходу роботи
Відповіді на контрольні запитання
Висновки за результатами роботи (обов’язково!!!)

_Conclusion_

This work provided an introduction to virtualization, hypervisor functionality, and the key features of the Linux operating system. Understanding hypervisors, both Type 1 and Type 2, is essential for managing virtual environments effectively.
VirtualBox, as a widely used Type 2 hypervisor, offers a flexible and user-friendly platform for creating, managing, and testing virtual machines. Additionally, the study of Linux-based virtualization solutions, such as KVM, highlights the advantages of open-source tools in optimizing system performance and resource allocation. Overall, virtualization plays a crucial role in modern computing, enhancing system efficiency, security, and scalability.
