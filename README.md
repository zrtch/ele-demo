# Vue 3 + Typescript + Vite

首次安装可能会出现报:Preprocessor dependency "sass" not found. Did you install it?
只需安装 node-sass 或 sass 即可解决

```
npm install node-sass
npm install sass --save-dev
```

## husky

```
npx husky install
npx husky add .husky/commit-msg "node scripts/verifyCommit.js"
```

## eslint

```
npm install -D eslint typescript

npm install -D  eslint-plugin-vue @vue/eslint-config-typescript

npm install -D @typescript-eslint/parser @typescript-eslint/eslint-plugin
npx husky add .husky/pre-commit "npm run lint"


```

@todo lint-staged 只校验暂存区
@todo pettier 配合 eslint 优化代码格式，这里忽略

```
npm install -D prettier eslint-plugin-prettier @vue/eslint-config-prettier
```

## unit test

https://github.com/vuejs/vue-test-utils-next

jest27 有点小问题，手动安装版本 26

```
npm install -D jest@26 vue-jest@next @vue/test-utils@next
npm install -D babel-jest@26 @babel/core @babel/preset-env
npm install -D ts-jest@26 @babel/preset-typescript @types/jest


```
