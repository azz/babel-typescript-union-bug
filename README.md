Run

```sh
npm i
npm t
```

```

> babel-typescript-bug@1.0.0 test /work
> babel index.ts

TypeError: Property types[0] of UnionTypeAnnotation expected node to be of a type ["FlowType"] but instead got "TSTypeAnnotation"
    at validate (/work/node_modules/@babel/types/lib/definitions/utils.js:128:13)
    at validator (/work/node_modules/@babel/types/lib/definitions/utils.js:97:7)
    at Object.validate (/work/node_modules/@babel/types/lib/definitions/utils.js:172:7)
    at validate (/work/node_modules/@babel/types/lib/validators/validate.js:17:9)
    at builder (/work/node_modules/@babel/types/lib/builders/builder.js:46:27)
    at UnionTypeAnnotation (/work/node_modules/@babel/types/lib/builders/generated/index.js:733:31)
    at Object.createUnionTypeAnnotation (/work/node_modules/@babel/types/lib/builders/flow/createUnionTypeAnnotation.js:20:47)
    at NodePath.ConditionalExpression (/work/node_modules/@babel/traverse/lib/path/inference/inferers.js:124:14)
    at NodePath._getTypeAnnotation (/work/node_modules/@babel/traverse/lib/path/inference/index.js:63:20)
    at NodePath.getTypeAnnotation (/work/node_modules/@babel/traverse/lib/path/inference/index.js:29:19)
npm ERR! Test failed.  See above for more details.
```
