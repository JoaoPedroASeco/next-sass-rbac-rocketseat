# Workspaces

- Utilizando TurboRepo para criar o projeto, iremos utilizar o workspace disponibilizado pelo npm para compartilhar dependencias entre si, para que não haja duplicação entres as dependencias.

- Para iniciar o projeto, foi criado uma pasta /config e dentro dessa pasta config ira ficar centralizado todas as configs de workspace e permissões de usuario.

- Foi adicionado ao package.json na propriedade "workspaces" a pasta "/config/\*":

```json
// /package.json
{
  // other properties
  "workspaces": ["apps/*", "packages/*", "config/*"]
}
```
