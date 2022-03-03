# Quasar App (testcascader)

A Quasar Framework app

## Install the dependencies

```bash
npm install
```

### Start the app in development mode (hot-code reloading, error reporting, etc.)

```bash
quasar dev
```

### Lint the files

```bash
npm run lint
```

### Format the files

```bash
npm run format
```

### Build the app for production

```bash
quasar build
```
<cascader
      label="单位"
      :options="data"
      dense
      optlabel="name"
      optvalue="id"
	  important
      @change="handleDeptIdChange"
    >
	
	组件提供了一个clearcascader方法来主
### Customize the configuration

See [Configuring quasar.conf.js](https://quasar.dev/quasar-cli/quasar-conf-js).
