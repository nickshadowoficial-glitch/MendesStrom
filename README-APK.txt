MENDES STROM — PROJETO ANDROID

Este pacote é um projeto Android nativo (WebView + Java) pronto para abrir no Android Studio e gerar o APK.

IMPORTANTE
- Este ambiente não possui Android SDK/build-tools, então não foi possível gerar um APK instalável aqui sem fingir que foi compilado.
- O app não substitui Defesa Civil/INMET.
- A previsão usa Open-Meteo e é previsão de modelo, não radar observado.
- O endereço do servidor de alertas fica em localStorage (mendesstrom_api). Para conectar ao servidor, abra o código index.html e defina a URL HTTPS do servidor, ou depois podemos transformar isso em configuração dentro do app.
- O servidor precisa ser o pacote mendes_strom_push_real.zip já criado anteriormente.
- Push nativo em segundo plano ainda precisa de Firebase Cloud Messaging (FCM) ou outro provedor nativo. O botão de notificações já solicita a permissão do Android.

COMO GERAR O APK
1. Instale o Android Studio em um computador.
2. Abra a pasta MendesStromAndroid.
3. Espere o Gradle sincronizar e baixar as dependências.
4. Use Build > Build APK(s).
5. O APK de debug aparecerá em app/build/outputs/apk/debug/app-debug.apk.

RECURSOS JÁ NO PROJETO
- Tela de aplicativo sem barras de navegador.
- Responsivo para celular e tablet.
- Localização aproximada via GPS/permissão Android.
- Previsão horária para Mendes.
- Timeline de até 48h.
- Mapa com chuva prevista e indicador de trovoada do modelo.
- Localidades verificadas para seleção, sem inventar coordenadas.
- Alertas do servidor filtrados por localidade ou Todo Mendes.
- Área Equipe protegida pelo login do servidor (senha padrão do servidor: 2013).
- Desenho de ponto/linha/polígono/retângulo/círculo no mapa da equipe.
- Telefones 199, 193, 192 e 190.
