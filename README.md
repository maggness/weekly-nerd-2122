# Weekly nerd

For the weekly nerd, every week a nerd comes to talk (surprise) about everything front-end. This is done by companies, former students, designers and professionals, often combinations of those!

## Learning goals
- Getting acquainted with the professional field
- Orientate on the field
- Learn to write subject-related articles

## Format of the readme:
[Articles](https://github.com/maggness/weekly-nerd-2122/edit/master/README.md#articles)

Weekly Nerd

Weekly Mingle

Reflection

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

You could also think of Typescript as a bit of a linter for JS, so you don't have to relearn much like with PureScript or CoffeeScript. And every JS file is compatible with TypeScript, you can therefore easily convert the JavaScript to TypeScript. There is a change that you will get typing errors, but it will still work.

To give some examples of some other types you have for example Void & Never. Void is used when no value will be returned, this is the opposite of Any.
``` typescript
let useless: void = undefined;
useless = 1; // error
```

Never is the return type for something that should never occur.
``` typescript
function raiseError(message: string): never {
    throw new Error(message);
}
```
Typescript is so big, the chance that I will use Typescript during my work & internship is very high. Really interesting to read about it and get started with it. Also, the fact that writing documentation becomes a lot less a part of writing your code is already a + for me!

https://www.typescriptlang.org/
https://www.stxnext.com/blog/typescript-pros-cons-javascript/
weekly-mingle-typescript-workshop (LabelA)
https://www.typescripttutorial.net/typescript-tutorial/typescript-void-type/
What is TypeScript and Should You Learn it?

## Article 2: Typescript
swag
