# Nardoto Editor: Extras

Loja de extras do [Nardoto Editor](https://github.com/LoopLess-nardoto/nardoto-editor-open).
O Editor lê o index.json deste repositório (aba **Extras**) e baixa os pacotes das releases.

- index.json: catálogo que o Editor lê (schema 1).
- Pacotes .driftpkg: anexados às releases, assinados com a chave Ed25519 da loja. O Editor
  recusa pacote sem assinatura válida.

Para publicar um extra novo, use scripts/loja/empacotar.mjs no repositório do Editor.
A chave secreta de assinatura nunca vai para este repositório.
