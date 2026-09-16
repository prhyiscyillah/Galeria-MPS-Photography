# Galeria de Entrega — MPS Photography

Site estático (HTML puro, sem build) para entregar as fotos finais do ensaio ao cliente,
em formato de mosaico visual (estilo Pinterest), com botão de download em cada foto.

Diferente do site de seleção (Firebase): aqui não existe login nem seleção — é só entrega.

## Como publicar (mesmo fluxo do site principal)

1. Suba a pasta inteira para um repositório no GitHub (pode ser um repo novo, ex: `Galeria-Entrega-MPS`,
   ou uma subpasta dentro do repo `Fotoalbum-MPS` — nesse caso ajuste o "Root Directory" no Vercel).
2. No Vercel: New Project → importe o repositório → Framework Preset: **Other** (é HTML puro, sem build).
3. Deploy. O Vercel vai te dar um link tipo `galeria-entrega-mps.vercel.app`.

## Como usar (depois de publicado)

- Link SEM parâmetro (ex: `seulink.vercel.app`) → abre o **painel** pra você criar uma galeria nova
  (cola nome do cliente, título, links das fotos, link da pasta do Drive pra "baixar tudo").
- Ao clicar em "Gerar link da galeria", ele monta um link tipo `seulink.vercel.app/?d=XXXXX`
  — esse `?d=` é o link que você envia pro cliente. Cada cliente tem um link diferente.
- Não precisa de banco de dados nem backend — todos os dados da galeria ficam guardados
  dentro do próprio link (por isso o link fica grande, isso é normal).

## Fotos

Continue hospedando as fotos como já faz (ImgBB, Google Drive etc — links do Drive são
convertidos automaticamente para link direto de imagem). Lembre de deixar o link/pasta
como "Qualquer pessoa com o link pode ver", senão a foto aparece quebrada pro cliente.
