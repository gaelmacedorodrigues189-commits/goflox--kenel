# Certificados Goflox 2026

A partir desta versão, o projeto contém a pasta:

`certificados/`

No boot, o kernel possui uma camada `certificate_store` preparada para procurar:

`/certificados/`

e o certificado raiz:

`/certificados/goflox-2026-root.conf`

A finalidade é permitir futuramente que o Driver Manager aceite somente drivers,
módulos e firmware que tenham uma assinatura confiável.

Isso é uma infraestrutura de confiança; os arquivos `.conf` incluídos são
configuração/metadados de desenvolvimento, não certificados criptográficos
válidos.
