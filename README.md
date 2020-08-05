# Docusaurus Plugin OpenAPI (WIP)

![](https://user-images.githubusercontent.com/4212769/85324376-b9e3d900-b497-11ea-9765-c42a8ad1ff61.png)

Install the plugin in your docusaurus project:
```
yarn add docusaurus-plugin-openapi
```

Add it as a plugin to `docusaurus.config.js`:
```js
plugins: [
  ["docusaurus-plugin-openapi", {
    openapiPath: require.resolve("./openapi.json"),
    sidebarLabel: "summary", // summary | operationId
    pageId: "summary", // summary | operationId
  }],
]
```

Add it as a link in `docusaurus.config.js` to `themeConfig.navbar.links`:
```js
{
  to: "api/",
  activeBasePath: "api",
  label: "API",
  position: "left",
}
```
