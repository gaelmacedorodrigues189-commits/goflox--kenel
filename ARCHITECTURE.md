# GOFLOX KERNEL 4.0 — Arquitetura Linux-inspired

O Goflox utiliza conceitos e uma organização de subsistemas inspirados no
Linux, mas não é uma cópia do Linux.

## Regra do projeto

- Linux: referência arquitetural e conceitual.
- Goflox: APIs, ABI, estruturas internas, Driver Manager, módulos, segurança,
  certificados e integração de hardware próprios.

O projeto NÃO copia código-fonte ou drivers Linux.

## Mapa

arch/        arquitetura da CPU
kernel/      processos, scheduler, syscalls e IPC
mm/          memória virtual, heap e allocator
drivers/     hardware e Driver Manager
fs/          VFS e sistemas de arquivos
net/         rede
security/    segurança
firmware/    firmware
modules/     módulos Goflox
init/        inicialização
certificados/ confiança Goflox 2026

## Linguagens

C       -> núcleo e interfaces de baixo nível
C++     -> Driver Manager e componentes orientados a dispositivos
Rust    -> segurança e componentes escolhidos para maior segurança de memória
Bash    -> build, empacotamento e ferramentas de sistema
Assembly -> entrada de boot e trechos dependentes da CPU

Python NÃO é usado no kernel.
