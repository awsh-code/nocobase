---
nav:
  title: API
  order: 3
toc: menu
---

# Application

## `app.db`

数据库实例，详情见 [Database API](database)

##### Definition

```ts
class Application {
  public db: Database;
}
```

##### Examples

```ts
app.db.on('xxx', () => {

});
```

## app.resourcer

资源实例

## app.pm

插件管理器，详情见 [Plugin Manager](plugin-manager)

##### Definition

```ts
class Application {
  public pm: PluginManager;
}
```

##### Examples

```ts
app.pm.enable(['plugin-name']);
```

## app.i18n

国际化，i18next 实例，详情见 [I18next API](https://www.i18next.com/overview/api)，在 Middleware 里请使用 [ctx.i18n](context#ctxi18n)

##### Definition

```ts
class Application {
  public i18n: I18next.i18n;
}
```

##### Examples

```ts
app.i18n.t('Hello');
```

## app.constructor()

构造器

## app.use()

中间件

## app.on()

事件

## app.emit()

## app.emitAsync()

## app.collection()

等同于 app.db.collection()

## app.actions()

等同于 app.resourcer.registerActions()

## app.resource()

等同于 app.resourcer.define()

## app.parse()

等同于 app.cli.parse()

## app.load()

加载配置

## app.init()

初始化

## app.start()

启动应用

## app.stop()

停止应用

## app.command()

等同于 app.cli.command()

## app.plugin()

等同于 app.pm.add()