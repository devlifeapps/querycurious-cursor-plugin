# QueryCurious para o Cursor

Plugin público do QueryCurious Lifeapps, no formato do [template de plugins do Cursor](https://github.com/cursor/plugin-template).

Quem instala pelo marketplace entra com o usuário do SSO Lifeapps. O `client_id` já está em `plugins/querycurious/mcp.json`. O repositório não contém segredo.

## Validar localmente

Copie o conteúdo de `plugins/querycurious` para `~/.cursor/plugins/local/querycurious` e rode **Developer: Reload Window**. Em **Customize**, conecte o servidor e faça login. O Cursor desktop usa o callback `http://localhost:8787/callback`.

## Conferir o template

```bash
node scripts/validate-template.mjs
```

## Publicar

Envie a URL pública deste repositório em [cursor.com/marketplace/publish](https://cursor.com/marketplace/publish).
