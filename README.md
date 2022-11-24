# Demostrating the issue of using the TypeScript 4.9 "satisfies" keyword with WebPack

## Running

    yarn
    yarn dev

    # In another terminal...
    yarn start

## Workaround

Inserting the missing dependency import names as bare evaluations forces the bundler to include the modules at runtime. See the top of `src/index.ts`.

Also, simply removing the `satisfies` keyword works.
