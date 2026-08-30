# CineMax TV — Instruções do projeto

O usuário quer que o assistente **sempre** ofereça sugestões de melhorias e
ideias para ajudar no aplicativo CineMax TV (app de TV em HTML/JS), a cada
tarefa/ajuste realizado. Sempre terminar as respostas com sugestões práticas.

## Contexto do projeto

- App de TV gratuito "CineMax TV" (HTML/JS), base 1280x720 com escala automática.
- Navegação por controle remoto (setas + Enter + Esc).
- Perfis de usuário locais (máx. 6) salvos em localStorage.
- Catálogo: 23 capas (2:3) em carrossel; avatares em avatars/.
- Cor da marca: roxa #8b5cf6. Splash com logo ▶ e som via Web Audio.
- Escala atual em fit() no index.html (overscan TV TCL).
- Versão atual: v2.6.6 (LEIA-ME.txt). Splash/rodapé devem ficar consistentes.
- Títulos das capas ids 0-4 conferidos; ids 5-22 dependem do usuário/ferramenta
  de análise de imagem (este modelo não lê imagens).