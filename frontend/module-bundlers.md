## Module Bundlers

A **module bundler** is a tool that takes many small files and **bundles** them into fewer (often one) optimized files that browsers can load efficiently. It is the logistics manager of your frontend world 📦⚙️

Modern apps may have hundreds of modules. Browsers prefer fewer network requests. Bundlers solve this mismatch.

---

## Why Module Bundlers Exist

Browsers were not always good at handling modules.

Problems bundlers solve:

- Too many files → slow page loads
- Different module systems (CommonJS, ES Modules)
- Need to transform code (TypeScript, JSX, SCSS)
- Need to optimize for production

---

## What a Bundler Does (Step by Step)

1. **Starts from an entry file**
   Example: `index.js`

2. **Builds a dependency graph**
   Follows `import` and `require` statements

3. **Transforms code**
   - TypeScript → JavaScript
   - JSX → JavaScript
   - SCSS → CSS

4. **Bundles modules together**
   Combines files into one or more output files

5. **Optimizes for production**
   - Minification
   - Tree shaking (remove unused code)
   - Code splitting
   - Asset hashing

6. **Outputs final files**
   Example:

   ```txt
   dist/
     app.3f9a2c.js
     vendor.a81d02.js
   ```

---

## Popular Module Bundlers

- Webpack
- Rollup
- Parcel
- Vite
- esbuild

---

## Module Bundler vs Transpiler

| Tool                    | Purpose                    |
| ----------------------- | -------------------------- |
| Bundler                 | Combines files + optimizes |
| Transpiler (Babel, SWC) | Converts syntax            |
| Minifier (Terser)       | Shrinks code               |

## References

- [Module Bundlers Explained](https://www.youtube.com/watch?v=5IG4UmULyoA)
