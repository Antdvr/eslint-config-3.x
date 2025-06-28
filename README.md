# @antdvr/eslint-config

- Antdv.pro 的 ESlint Config 插件
- Only Support ESlint v9.x

## How to Use it

- Install

  ```bash
    pnpm add @antdvr/eslint-config-3.x
  ```

- Usage

  a. Using (default)

  ```typescript
    import antdvr from '@antdvr/eslint-config-3.x'

    export default [
      ...antdvr.configs['flat/recommended'],

      // eg. ....
      {
        {
          rules: {
            // Custom rules
          }
        }
      }
    ]
  ```

  b. Using by tseslint

  ```typescript
  import tseslint from "typescript-eslint";
  import antdvr from "@antdvr/eslint-config-3.x";

  export default tseslint.config({
    extends: [...antdvr.configs["flat/recommended"]],
  });
  ```
