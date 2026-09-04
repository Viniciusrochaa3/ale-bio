# Bio da Ale — clone do Beacons (tema preto)

## Arte
`assets/hero.jpg` — a arte "ALE SCHERER" (1086x1448). Para trocar, é só
substituir o arquivo mantendo o mesmo nome e proporção (3:4 aproximado).
Se a proporção mudar, ajuste o `aspect-ratio` no CSS do `.hero img`.

## O que tem na página
- Arte no topo (sem o texto "aleslots.ofc")
- Legenda: "Confira todas as casas que eu jogo 🚀"
- Ícone do Instagram (@aleslotss)
- Os 10 links, **exatamente as mesmas URLs do Beacons**, na mesma ordem
- Pop-up +18 antes de entrar nas casas — o nome muda conforme a casa
- Rodapé com selo de SSL + aviso legal de jogo responsável

## Mexer nos links
Tudo fica no array `LINKS` dentro do `index.html` (perto do fim).
- `gate:true`  → mostra o pop-up +18
- `casa:"..."` → nome que aparece no pop-up
- `gate:false` → abre direto (WhatsApp, Telegram, Instagram, YouTube)

## Pop-up: quantas vezes pergunta
Pergunta 1x por visita (guarda no `sessionStorage`).
Para perguntar sempre, apague a linha `marcarConfirmado();` no `ovYes`.

## Selo SSL
O selo verde só acende quando o site está publicado em HTTPS.
Rodando local ele mostra "PRÉ-VISUALIZAÇÃO LOCAL" — é o comportamento certo.

## Publicar
Mesmo esquema dos outros: sobe a pasta no GitHub Pages e aponta o domínio.
