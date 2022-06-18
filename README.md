# Articles
## Article 1: Typescript

TypeScript is an open-source programming language developed by Microsoft that complies to JavaScript. Typescript builds on Javascript so that it is easier and better for developers to keep an overview. You also need less documentation because the code actually documents itself.

Everything you can write with Javascript can also be written with Typescript, this is because the Javascript does not change but builds on it. You can also easily use it with React, for example.

With Typescript you indicate what you are going to use the data for, for example that it is a number, string, boolean. This way you can't accidentally put a string where there should actually be a number. Here's a small example of defining types:

``` typescript
 // number
  let cookiesCount: number = 68;

  // string
  let teach: string = ‘Example’;

  // boolean
  let typescriptUsed: boolean = true;

  // Array of strings (using the [] syntax)
  let years: string[] = [‘1969’, ‘2001’, ‘2021’, ‘3333’];

  // Object with properties 'id' and 'name' and value of type string
  let person: {
    name: string = ‘Tim’,
    id: string = ‘AF5SA335AA2’
  };
```
