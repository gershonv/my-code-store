## vscode 利器

- JavaScript (ES6) code snippets
- Reactjs code snippets
- React/Redux/react-router Snippets

### js

#### import

- `imp` => `import moduleName from 'module'` - imports entire module
- `imn` => `import 'module'` - imports entire module without module name
- `imd` => `import {} from 'module'` - imports only a portion of the module using destructing

react:

- `imr` => `import React from 'react'`
- `imrc` => `import React, { Component } from 'react'`
- `impt` => `import PropTypes from 'prop-types'`
- `imconnect` => `import { connect } from 'react-redux'`
- `improvider` => `import { Provider } from 'react-redux'`
- `imrr` => `import { BrowserRouter, Route } from 'react-router-dom'`

#### export

- `mde` => `module.exports = {}` - default module.exports
- `enf` => `export const functionName = params => {}` - exports name function
- `edf` => `export default params => {}` - exports default function
- `rat` => `export const = ''` - Redux actionCreator

#### methods

- `anfn` => `(params) => {}` - creates an anonymous function
- `nfn` => `const add = (params) => {}` - creates a named function
- `dob` => `const {rename} = fs` - 结构赋值
- `thenc` => `.then((res) => {).catch((err) => {})` - adds then and catch declaration to a promise

### react

- `rcc` - class component skeleton

```jsx
import React, { Component } from 'react'

class componentName extends Component {
  render() {
    return <div />
  }
}

export default componentName
```

- `rccp` - class component skeleton with prop types after the class

```jsx
import React, { Component, PropTypes } from 'react'

class componentName extends Component {
  render() {
    return <div />
  }
}

componentName.propTypes = {}

export default componentName
```

- `rsc` - stateless component skeleton
  - 同上 `rscp` 增加验证

```jsx
import React from 'react'

const componentName = () => {
  return <div />
}

export default componentName
```

#### 生命周期

- `cwm`→ `componentWillMount`
- `cdm`→ `componentDidMount`
- `cwr`→ `componentWillReceiveProps`
- `scu`→ `shouldComponentUpdate`
- `cwup`→ `componentWillUpdate`
- `cdup`→ `componentDidUpdate`
- `cwun`→ `componentWillUnmount`
- `cdc`→ `componentDidCatch`

#### propTypes

- `impt` => `import PropTypes from 'prop-types'`
- `spt` => `static propTypes = {}`
- `pta` => `PropTypes.array`
- `ptar` => `PropTypes.array.isRequired`
  - `pt` 同理（略）

#### Redux

- `rac` - Redux actionCreator

```jsx
export const actionCreator = payload => ({
  type: actionType,
  payload
})
```

- `mspt` - `const mapStateToProps = (state, ownProps) => ({})`
- `conntect` - `export default connect(mapStateToProps, mapDispatchToProps)(containerName)`

---

其他

- `route` => `<Route path='path' component={component}/>`
- `navlink` => `<NavLink to={path}>{anchorText}</NavLink>`
- `router` => `<Router></Router>`

### setting.json

个人 vscode 配置

```json
{
  "window.menuBarVisibility": "default",
  // 右侧代码预览框
  "editor.minimap.enabled": false,
  "git.autofetch": true,
  "explorer.confirmDelete": false,
  // 避免卡死
  "search.followSymlinks": false,
  // 修改文件时修改各个文件的 import 路径
  "javascript.updateImportsOnFileMove.enabled": "always",
  // react html 自动补全
  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  },
  // 单引号
  "prettier.singleQuote": true,
  // 去掉代码结尾的分号
  "prettier.semi": false,
  // 代码间距
  "prettier.tabSize": 2,
  // 宽度 120 时换行
  "prettier.printWidth": 120
}
```

## google 插件

- 代理大师(Google Edition)
- AdGuard 广告拦截器
- Octotree
  - github 辅助工具
- React Developer Tools
- Redux DevTools
- Tampermonkey
  - 破解网盘
