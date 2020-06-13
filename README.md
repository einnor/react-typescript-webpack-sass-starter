## Getting Started

- `git clone <REPO_NAME>`
- `yarn`

### To allow import of SASS modules

- `mkdir src/typings`
- `touch src/typings/scss.d.ts`
- Add the below code to `scss.d.ts`

```
  // scss.d.ts
  declare module '*.css' {
    const content: { [className: string]: string; };
    export default content;
  }
  declare module '*.scss' {
    const content: { [className: string]: string; };
    export default content;
  }
```

## Runnning in Development

- `yarn run dev`

## Runnning in Production

- `yarn run build` to generate bundled app in `dist`
