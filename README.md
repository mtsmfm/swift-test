# graphql-codegen-swift-operations

[graphql-codegen](https://graphql-code-generator.com/) Swift plugin for GraphQL operations.

## Demo

You can find example project on /swift-test-project dir:

https://github.com/mtsmfm/graphql-codegen-swift-operations/tree/master/swift-test-project

Generated file:

https://github.com/mtsmfm/graphql-codegen-swift-operations/blob/master/swift-test-project/Sources/app/generated.swift

Operation:

https://github.com/mtsmfm/graphql-codegen-swift-operations/blob/master/swift-test-project/query.graphql

Usage:

https://github.com/mtsmfm/graphql-codegen-swift-operations/blob/master/swift-test-project/Sources/app/main.swift

## How to use

To install graphql-codegen, follow the

https://graphql-code-generator.com/docs/getting-started/installation

### 1. Install this package

```
$ yarn add -D @mtsmfm/graphql-codegen-swift-operations
```

or

```
$ npm install --save-dev @mtsmfm/graphql-codegen-swift-operations
```

### 2. Write codegen.yml

It'll be like the following:

```yaml
schema: https://swapi.graph.cool/graphql
documents: 'query.graphql'
generates:
  Sources/app/generated.swift:
    - '@mtsmfm/graphql-codegen-swift-operations'
```

### 3. Generate Swift files

```
$ graphql-codegen
```

## TODOs

- InlineFragment
- Nullable array
- Union
- Add some other stuff to scalar map
- Customizable scalar map
