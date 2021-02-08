## module version list

```json
// about typescript
"typescript": "^4.1.3",
```

```json
// about webpack
"clean-webpack-plugin": "^3.0.0",
"@types/mini-css-extract-plugin": "^1.2.2",
"css-loader": "^5.0.1",
"html-webpack-plugin": "^5.0.0",
"mini-css-extract-plugin": "^1.3.5",
"webpack": "^5.21.2",
"webpack-cli": "^4.5.0",
"webpack-dev-server": "^3.11.2"
```

```json
// about babel
"@babel/core": "^7.12.13",
"@babel/preset-env": "^7.12.13",
"@babel/preset-react": "^7.12.13",
"@babel/preset-typescript": "^7.12.13",
"babel-loader": "^8.2.2",
```

```json
//about react

"react": "^17.0.1",
"react-dom": "^17.0.1"
"@types/react": "^17.0.1",
"@types/react-dom": "^17.0.0",
```

### Webpack Plugins

- html-webpack-plugin :
  - 따로 분리하여 번들한 css파일과 js파일을 각각 html 파일에 link 태그,
    script태그로 추가해줘야 한다. HtmlWebpackPlugin은 이것을 자동화 해준다.
- clean-webpack-plugin
  - 빌드 이전 결과물을 제거하는 플러그인으로 빌드 결과물은 웹팩에서
    아웃풋 경로에 설장한 곳으로 폴더 및 파일들이 모이는데 빌드 했을시 이전 빌드내용이 삭제되지 않고
    그대로 남아있는 경우도 있어 이것을 해결해주는 플러그인이다.
- mini-css-extract-plugin
  - style-loader 대체로 사용 가능
    css 파일들을 하나로 합침
    loader를 대체하므로 plugins와 use에 모두 적용

### Babel

- babel-loader
  - 바벨과 웹팩을 연결
- @babel/core
- @babel/preset-env
  - 브라우저에 필요한 ecmascript 버전을 자동으로 파악해서 알어서 polyfill을 넣어줌
- @babel/preset-react
  - JSX와 같은 파일을 지원
- @babel/preset-typescript
  - typsecript 지원
