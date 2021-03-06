# Snapshot report for `test/test.js`

The actual snapshot is saved in `test.js.snap`.

Generated by [AVA](https://avajs.dev).

## Task basic behavior

> fixtures/expected/basic.js

    `const answer = 42;␊
    ␊
    const foo = "bar";␊
    ␊
    console.log(foo + answer);␊
    `

## With multiple files input

> fixtures/expected/_basic.js

    `const answer = 42;␊
    ␊
    const foo = "bar";␊
    ␊
    console.log(foo + answer);␊
    `

> fixtures/expected/_second.js

    `console.log("second");␊
    `

## With plugin array

> fixtures/expected/plugin1.js

    `␊
    // ok␊
    const answer = 42;␊
    ␊
    const foo = "bar";␊
    ␊
    console.log(foo + answer);␊
    `

> fixtures/expected/plugin2.js

    `␊
    // ok␊
    const answer = 42;␊
    ␊
    const foo = "bar";␊
    ␊
    console.log(foo + answer);␊
    `

## With plugin function

> fixtures/expected/plugin1.js

    `␊
    // ok␊
    const answer = 42;␊
    ␊
    const foo = "bar";␊
    ␊
    console.log(foo + answer);␊
    `

> fixtures/expected/plugin2.js

    `␊
    // ok␊
    const answer = 42;␊
    ␊
    const foo = "bar";␊
    ␊
    console.log(foo + answer);␊
    `

## With source map

> fixtures/expected/sourcemap.js

    `const answer = 42;␊
    ␊
    const foo = "bar";␊
    ␊
    console.log(foo + answer);␊
    ␊
    //# sourceMappingURL=sourcemap.js.map`

> fixtures/expected/sourcemap.js.map

    '{"version":3,"file":"_basic.js","sources":["fixtures/_module.js","fixtures/_basic.js"],"sourcesContent":["const answer = 42;\\n\\nexport default answer;\\n\\nexport const unused = \\"foo\\";\\n","import answer from \\"./_module\\";\\n\\nconst foo = \\"bar\\";\\n\\nconsole.log(foo + answer);\\n"],"names":[],"mappings":"AAAA,MAAM,MAAM,GAAG,EAAE;;ACEjB,MAAM,GAAG,GAAG,KAAK,CAAC;AAClB;AACA,OAAO,CAAC,GAAG,CAAC,GAAG,GAAG,MAAM,CAAC,CAAC"}'

## With source map inline

> fixtures/expected/sourcemap-inline.js

    `const answer = 42;␊
    ␊
    const foo = "bar";␊
    ␊
    console.log(foo + answer);␊
    ␊
    //# sourceMappingURL=data:application/json;charset=utf-8;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiX2Jhc2ljLmpzIiwic291cmNlcyI6WyJmaXh0dXJlcy9fbW9kdWxlLmpzIiwiZml4dHVyZXMvX2Jhc2ljLmpzIl0sInNvdXJjZXNDb250ZW50IjpbImNvbnN0IGFuc3dlciA9IDQyO1xuXG5leHBvcnQgZGVmYXVsdCBhbnN3ZXI7XG5cbmV4cG9ydCBjb25zdCB1bnVzZWQgPSBcImZvb1wiO1xuIiwiaW1wb3J0IGFuc3dlciBmcm9tIFwiLi9fbW9kdWxlXCI7XG5cbmNvbnN0IGZvbyA9IFwiYmFyXCI7XG5cbmNvbnNvbGUubG9nKGZvbyArIGFuc3dlcik7XG4iXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6IkFBQUEsTUFBTSxNQUFNLEdBQUcsRUFBRTs7QUNFakIsTUFBTSxHQUFHLEdBQUcsS0FBSyxDQUFDO0FBQ2xCO0FBQ0EsT0FBTyxDQUFDLEdBQUcsQ0FBQyxHQUFHLEdBQUcsTUFBTSxDQUFDLENBQUMifQ==`

## With src and dest config

> fixtures/expected/target.js

    `const answer = 42;␊
    ␊
    const foo = "bar";␊
    ␊
    console.log(foo + answer);␊
    `
