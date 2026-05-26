# Video Template Editor

Ferramenta para sobrepor vídeos em um template de imagem 9:16 — processamento 100% no navegador, sem envio de dados para servidores.

## Como usar

1. Faça upload do template PNG/JPG (formato 9:16 recomendado)
2. Ajuste a safe zone no canvas (arraste ou redimensione)
3. Faça upload dos vídeos (MP4 ou MOV)
4. Clique em **Processar** e baixe os vídeos gerados

## Tecnologias

- **WebCodecs API** — codificação H.264 + AAC nativa do browser
- **mp4-muxer** — gera MP4 padrão com `moov` no início (compatível com WhatsApp/iOS/Android)
- **Web Audio API** — captura áudio sem eco nos alto-falantes
- **Canvas 2D** — composição de frames e editor visual de safe zone

## Requisitos

- Chrome 94+ (ou Edge 94+) — necessário para WebCodecs API

## Deploy

Site estático — sem backend, sem banco de dados.
Hospedado via [Vercel](https://vercel.com).

## Privacidade

Nenhum dado é enviado para a internet. Todo o processamento ocorre localmente no navegador do usuário.
