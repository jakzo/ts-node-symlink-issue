# ts-node symlink issue

1. Run: `yarn`
   - This will create a symlink of `node_modules/b -> packages/b`
2. Run: `yarn ts`
   - This will complete successfully
3. Run: `yarn ts-node`
   - This will result in an error in `packages/b/index.ts`: `Duplicate identifier 'X'.`
