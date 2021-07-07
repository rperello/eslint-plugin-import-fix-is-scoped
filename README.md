# eslint-plugin-import-fix-is-scoped

This is a fork of [eslint-plugin-import](https://www.npmjs.com/package/eslint-plugin-import).

**For all rule documentation and funding options please see that original package.**

This fork enables auto-fix sorting of imports even when there is an unassigned import in the midst. This change fails lots of tests and I haven't bothered to fix them all, so **be warned**. If you have issues, just use the original package linked above.

# What it is fixing

A problem with detecting as scoped module imports like

```js
import UnitDevice from '@/components/UnityDevice'
```

Is is a temporary solution until https://github.com/benmosher/eslint-plugin-import/pull/2146 is merged

To use this you must add the `import-fix-is-scoped` plugin to your eslintrc instead of `import`. Also, all rules must use the `import-fix-is-scoped/` path instead of `import/`.
