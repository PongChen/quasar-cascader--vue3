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
npm install  quasar-cascader-vue3 --save

import cascader from "quasar-cascader-vue3"

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
  handleDeptIdChange返回了选中的name和id// [name,id]
### Customize the configuration

See [Configuring quasar.conf.js](https://quasar.dev/quasar-cli/quasar-conf-js).
