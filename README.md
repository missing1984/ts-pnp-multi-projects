## setup

```
pushd ts && yarn && popd
pushd project-a && yarn && popd
pushd project-c && yarn && popd
```


## Problem 

Step 1

open project-a/index.ts, hover "react", vscode points the source to
```
module "xx/yarn-ts-multi-root/project-a/.yarn/cache/@types-react-npm-17.0.27-96dcc0d27b-3a1147d963.zip/node_modules/@types/react/index"
```

Step 2

open project-c/index.ts, hover "react", vscode still points the source to project-a
```
module "xx/yarn-ts-multi-root/project-a/.yarn/cache/@types-react-npm-17.0.27-96dcc0d27b-3a1147d963.zip/node_modules/@types/react/index"
```

I am expecting the step 2 would point me to the right source file.