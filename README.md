# Nova IPTV Player

Um player IPTV simples, em português, que roda diretamente no navegador. Importe uma playlist M3U/M3U8 local para organizar canais ao vivo, filmes e séries, pesquisar itens e tentar reproduzir streams compatíveis.
<img width="1852" height="892" alt="image" src="https://github.com/user-attachments/assets/7f75dec7-b534-4853-baa0-64ddb61dcd9a" />


## Como usar

1. Abra [`index.html`](./index.html) em um navegador atualizado.
2. Selecione **Adicionar Playlist** e escolha um arquivo `.m3u`, `.m3u8` ou `.txt`.
3. Navegue pelas categorias, use a busca ou selecione um item para abrir o player.

O atalho `Ctrl K` (ou `Cmd K` no macOS) foca a busca. A playlist carregada é salva no armazenamento local do navegador, quando permitido, para ser recuperada em uma visita futura nesse mesmo navegador.

## Compatibilidade

- HLS (`.m3u8`) é reproduzido com suporte nativo do navegador ou, quando necessário, com HLS.js carregado do jsDelivr.
- Streams MPEG-TS (`.ts` ou `.m2ts`) podem usar mpegts.js, também carregado do jsDelivr.
- A reprodução depende do formato e dos codecs aceitos pelo navegador e do acesso permitido pelo servidor do stream. Restrições de CORS ou de rede podem impedir o carregamento.
- Os recursos **Guia EPG**, **Catch Up**, **Gravações**, **Transferências**, **Multi-vista** e **Suas playlists** ainda não estão implementados.

## Privacidade e uso responsável

A playlist é selecionada como arquivo local e armazenada no navegador; o projeto não envia o arquivo a um servidor próprio. Os endereços de logos e streams podem ser acessados pelo navegador, e as bibliotecas de reprodução são obtidas do jsDelivr quando necessárias.

Use somente playlists e streams que você tem autorização para acessar.

## Tecnologias

- HTML, CSS e JavaScript, sem etapa de build ou instalação.
- HLS.js e mpegts.js carregados sob demanda via CDN para formatos que não tenham suporte nativo.
