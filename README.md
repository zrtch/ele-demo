# Vue 3 + Typescript + Vite

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
@todo pettier配合eslint优化代码格式，这里忽略

``` 
npm install -D prettier eslint-plugin-prettier @vue/eslint-config-prettier
```


## unit test
https://github.com/vuejs/vue-test-utils-next

jest27有点小问题，手动安装版本26

``` 
npm install -D jest@26 vue-jest@next @vue/test-utils@next 
npm install -D babel-jest@26 @babel/core @babel/preset-env 
npm install -D ts-jest@26 @babel/preset-typescript @types/jest


```