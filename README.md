1. Verificar se existe um **Development Team** associado ao aplicativo. Para isso, no painel com os arquivos, procure e clique no arquivo de projeto, clique em **All** nos filtros e digite **team** na busca. Você pode preencher o campo se estiver vazio;
2. Adicionar um texto descritivo sobre como a câmera é usada no app. Para isso, procure o arquivo ```Info.plist``` e adicione uma row do tipo Privacy - Camera Usage Description, acho que é esse o nome;
3. Verifique se o **Bundle Version** é maior que quaisquer bundle versions que tenhamos enviado anteriormente. Para isso, é preciso acessar o iTunes Connect e verificar quais bundles já foram enviados. Se necessário, trocar para um bundle maior;
4. Verificar se existe o warning **Update to Recommended Settings**. Se sim, aceitar a atualização para as configurações recomendadas.
5. Verifique se o **Bundle Identifier** está correto;
6. Gerar o archive do aplicativo. Para isso, ir no menu **Product > Archive**;
7. Se você estiver usando uma versão GM do macOS Sierra, será necessário mudar o ID do sistema operacional de compilação. Para isso:
  1. Clique em **Window > Organizer** e procure o archive gerado;
  2. Clique com o botão direito no archive e escolha **Show in Finder**;
  3. Clique com o botão direito no arquivo do aplicativo e escolha **Mostrar conteúdo do pacote**;
  4. Navegue até **Products > Applications**;
  5. Mais uma vez, clique com o botão direito no arquivo do aplicativo e escolha **Mostrar conteúdo do pacote**;
  6. Procure o arquivo ```Info.plist``` e edite no XCode;
  7. Troque o valor de ```BuildMachineOSBuild``` para ```15G31```;
8. Acessar o iTunes Connect e verificar - e se necessário alterar - descrição do app;
9. Subir app.
10. #oremos
