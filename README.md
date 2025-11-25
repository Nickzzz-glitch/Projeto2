# Aplicação da Prova de Integridade — essência da solução em blockchain

App estático (HTML + JS) que:
- Calcula **SHA-256** de arquivos **localmente** (sem upload).
- Gera um **recibo JSON** com hash, tamanho, nome, data/hora, emissor/nota.
- **Verifica** um arquivo contra um recibo, inteiramente offline.
- Mantém um **registro local** no navegador (localStorage).

## Como usar
1. Abra `index.html`.
2. Seção 1: escolha um arquivo → **Calcular SHA-256**.
3. Seção 2: preencha emissor/nota (opcional) → **Gerar & baixar recibo** (.json).
4. Seção 3: carregue o **recibo** e o **arquivo** → **Verificar**.

## Observações
- Isso captura a "essência": hash como prova de integridade e recibo assinável/armazenável.
- Em produção, você poderia:
  - Assinar o recibo digitalmente (ex.: ICP-Brasil, WebCrypto) — opcional.
  - Ancorar o hash num registro público (blockchain ou timestamp authority) — opcional.
