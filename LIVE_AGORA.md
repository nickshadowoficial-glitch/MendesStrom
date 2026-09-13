# Mendes Strom — sincronização ao vivo

Esta versão faz o que foi pedido no aplicativo:

- Moderador entra com **2013**.
- O alerta é enviado para um **servidor central**, não para `localStorage`.
- Os outros celulares consultam o servidor automaticamente a cada **15 segundos**.
- Ao abrir o aplicativo, o alerta ativo aparece no topo da tela.
- Não há push notification.
- Se o servidor estiver indisponível, o aplicativo informa que o alerta **não foi publicado**; ele não finge que sincronizou.

## Importante
O endereço configurado é `https://mendesstrom-live-api.onrender.com`, mas o servidor precisa estar realmente implantado no Render antes de a sincronização entre celulares funcionar.

Não gere um novo APK até o servidor estar online. Depois que `/api/health` responder, gere **um único APK** desta pasta.
