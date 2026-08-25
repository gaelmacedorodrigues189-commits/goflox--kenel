# Goflox Kernel 3.0

Kernel experimental do Goflox usando SOMENTE:

- C
- C++
- Rust
- Bash
- Assembly para a entrada de boot

Python NÃO faz parte do kernel nem do sistema de drivers.

## Funções

- núcleo em C
- Driver Manager em C++
- subsistema de hardware/segurança em Rust
- drivers Intel/AMD/NVIDIA
- estrutura para rede, armazenamento e entrada
- catálogo de compatibilidade
- módulos `.gkm`
- initramfs
- script Bash de compilação e instalação

## Arquitetura

Boot Assembly
    ↓
C Kernel
    ↓
Rust subsystems
    ↓
C++ Driver Manager
    ↓
PCI/USB/ACPI
    ↓
Vendor ID + Device ID
    ↓
Intel / AMD / NVIDIA / outros
    ↓
Driver nativo Goflox

## Importante

Drivers Linux `.ko`, Windows `.sys/.inf` e drivers proprietários não podem ser
carregados diretamente. Eles precisam de uma implementação/port para a API do
Goflox.

O projeto cria a infraestrutura para isso.


## 4.0 — Base inspirada no Linux

A organização dos diretórios e a separação dos subsistemas são inspiradas
na arquitetura do Linux, conforme o guia fornecido. O código, as interfaces
do kernel, o Driver Manager, o sistema de módulos e a infraestrutura de
certificados são próprios do Goflox.
