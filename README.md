Reproduction for an issue in VTI. Project was created with `npm init @vitejs/app` and then stripped of extra dependencies

### Reproduction steps
1. Pull repo and install deps
2. Run `npx vti diagnostics` in the root folder

### Expected
No errors, all types are valid

### Actual
```
File : ./src/components/HelloWorld.vue:1:1
Error: Cannot find name 'TestInterface'.
> 1 | <template>
    | ^
  2 |   <h1>{{ msg }}</h1>
  3 |   <test :test="{ key: 'test' }" />
  4 |   <p>
```