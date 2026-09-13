# Mendes Strom — modo AO VIVO

Esta versão deixa os alertas centralizados: moderador publica no servidor e os demais aparelhos consultam o mesmo servidor.

## Render + GitHub
1. Suba a pasta `ms_work` para um repositório GitHub.
2. No Render, crie um Blueprint usando `render.yaml`.
3. Informe `TEAM_PASSWORD` como `2013` (ou outra senha escolhida).
4. O Render criará o web service `mendesstrom-live-api` e o Postgres `mendesstrom-db`.
5. O endereço esperado do serviço, se o nome estiver disponível, será `https://mendesstrom-live-api.onrender.com`.
6. O APK já está configurado para consultar esse endereço.

O endereço `onrender.com` é público. O Render informa que web services recebem um subdomínio público próprio. O Blueprint também cria um Postgres para que os alertas não dependam do armazenamento local do telefone.

## Importante
- O APK precisa ser recompilado depois desta alteração.
- O código não usa mais `localStorage` para publicar alertas.
- Sem o backend publicado, não há sincronização entre telefones.
- Não prometa notificações push: isso é uma etapa separada.
