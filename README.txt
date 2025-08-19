NFC Gift – Kit Mocre (inspirado em Hold Me Tight)

Personalização aplicada:
- Título: "Kit Mocre"
- Frase revelada: "Obrigado por fazer parte da minha vida."
- Música: coloque "Thiaguinho – Falta Você" como MP3 em assets/audio.mp3 (opcional).

O que vem neste pacote:
- index.html  → página com “cadeado” (senha) e conteúdo revelado.
- assets/foto.jpg → imagem de exemplo (troque pela sua).
- (opcional) assets/audio.mp3 → adicione o seu MP3 curto aqui.
- README.txt → este guia.

1) Defina a senha (hash SHA-256)
   - Abra o arquivo index.html no navegador com ?setup=1 no final, por ex.:
     file:///SEU_CAMINHO/index.html?setup=1
   - Use o painel “Gerar Hash” para digitar sua senha (ex.: o nome dela em japonês) e copie o SHA-256 gerado.
   - Abra index.html num editor e cole o valor em PASSWORD_HASH.

2) Personalize
   - Substitua assets/foto.jpg pela sua imagem (mesmo nome).
   - (Opcional) coloque assets/audio.mp3 (a página detecta e mostra o player).
   - (Opcional) altere a constante PLAYLIST_URL para uma playlist sua.

3) Teste localmente
   - Abra index.html, digite a senha e veja se desbloqueia.

4) Publique (para usar no NFC)
   - Netlify Drop (simples): arraste a pasta /nfc_gift_kit_mocre para o serviço e pegue a URL.
   - GitHub Pages / Vercel também funcionam (site estático).

5) Gravar a tag (Android)
   - App "NFC Tools" → Gravar → Adicionar registro → URL → cole a URL pública → Gravar.

Roteiro de entrega (leve):
   “Quis te dar isso porque me lembrou da gente de um jeito bom. Sem peso nenhum.”

Observações de segurança:
   - A validação de senha ocorre no navegador (client-side), sem envio a servidores.
   - O hash protege a senha de estar em texto puro, mas não é uma proteção forte contra análise técnica.