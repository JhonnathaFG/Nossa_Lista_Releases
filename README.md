# Nossa Lista: APKs assinados

Este repositório público distribui apenas APKs assinados e os metadados necessários para a atualização do app. O código e a chave privada de assinatura ficam no repositório privado do aplicativo ou fora do GitHub.

Para publicar uma nova versão:

1. Gere e assine o APK com a mesma chave das versões anteriores. A versão interna e o `versionCode` precisam aumentar.
2. Crie um **rascunho** de Release com tag `vX.Y.Z`.
3. Anexe `Nossa-Lista-X.Y.Z.apk` antes de clicar em **Publish release**.
4. Confira na aba **Actions** se **Indexar APK assinado** terminou com sucesso e adicionou `release.json` ao Release.

O app consulta a versão uma vez por dia ao abrir e também pelo botão de verificação nas Configurações. O download e a instalação pedem confirmação no aparelho. Se o APK for anexado após a publicação, uma verificação programada tenta indexá-lo em até seis horas. A publicação como rascunho com o APK anexado gera o índice imediatamente. Se uma verificação programada estiver desativada após um período longo sem atividade, use **Indexar APK assinado** em Actions.
