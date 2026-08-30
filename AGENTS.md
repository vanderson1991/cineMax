# CineMax TV — Instruções do projeto

O usuário quer que o assistente **sempre** ofereça sugestões de melhorias e
ideias para ajudar no aplicativo CineMax TV (app de TV em HTML/JS), a cada
tarefa/ajuste realizado. Sempre terminar as respostas com sugestões práticas.

REINÍCIO APÓS DESLIGAMENTO: se o PC desligar/dormir no meio de uma tarefa,
ao voltar, **continuar exatamente de onde parou** sem recomeçar do zero.
Verificar primeiro o que já foi concluído (ex: git log, arquivos existentes,
o que foi publicado) e retomar o passo pendente.

## Contexto do projeto

- App de TV gratuito "CineMax TV" (HTML/JS), base 1280x720 com escala automática.
- Navegação por controle remoto (setas + Enter + Esc).
- Perfis de usuário locais (máx. 6) salvos em localStorage.
- Catálogo: 23 capas (2:3) em carrossel; avatares em avatars/.
- Cor da marca: roxa #8b5cf6. Splash com logo ▶ e som via Web Audio.
- Escala atual em fit() no index.html (overscan TV TCL).
- GitHub: repositorio publico `vanderson1991/cineMax` (branch master).
  Web/auto-update: https://vanderson1991.github.io/cineMax/
  Download: /download.html  | version.json controla versão (atual: 2.78).
- O modelo NAO le imagens: titulos das capas 5-22 dependem do usuario.
- Build do APK local: pasta `C:\Users\AppData\Local\Temp\opencode\apkbuild`
  (projeto em Cine-2024-APK, classes em out/, keystore cinematic = cinemax123).
  Commands: aapt2 compile/link, javac, d8, jar uf classes.dex, zipalign, apksigner.
  ATENCAO: assets devem ser adicionados com caminho `assets/www/...` usando "/"
  (nao "\") — no build de 30/08 a tela ficava preta por assets com barra invertida.
- O APK novo (v2.78) foi assinado com keystore NOVA (diferente da plataforma
  antiga). Para atualizar quem tem a versao antiga e preciso desinstalar antes.
- Títulos das capas ids 0-4 conferidos; ids 5-22 dependem do usuário/ferramenta
  de análise de imagem (este modelo não lê imagens).