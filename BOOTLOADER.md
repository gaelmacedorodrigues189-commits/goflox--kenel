# Goflox 4.3 — Bootloader

Adicionado um bootloader próprio ao kernel.

Ele é responsável por iniciar a máquina, preparar o ambiente inicial e
entregar o controle ao kernel. A árvore também mantém GRUB/Multiboot2 como
caminho de compatibilidade para testes.

Próxima evolução:
- BIOS completo;
- UEFI;
- leitura de filesystem;
- carregamento do kernel a partir do disco;
- passagem de mapa de memória;
- seleção de resolução/framebuffer;
- verificação dos certificados Goflox 2026 antes do carregamento do kernel.
