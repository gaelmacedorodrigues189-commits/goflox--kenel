# Referência arquitetural

O guia fornecido pelo usuário organiza o Linux em áreas como `arch/`,
`drivers/`, `fs/`, `kernel/`, `mm/`, `net/`, `security/`, `init/` e outras.

O Goflox adota uma separação semelhante porque ela facilita a manutenção e a
evolução do kernel. Entretanto, as implementações são próprias do Goflox.

A arquitetura de drivers também segue o conceito:

Hardware -> barramento -> identificação -> Driver Manager -> driver -> API do Kernel

A implementação Goflox deve permanecer independente da ABI do Linux.
