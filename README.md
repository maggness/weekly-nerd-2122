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

## Article 2: 3D in CSS

CSS is often not seen as a powerful programming language, but it certainly is. You have counters, variables, logic, compatibility tools and much more. You can also do super cool things with 3D: from making a full 3D object that you can rotate around to very smooth 3D buttons that move a bit with when you hover, it makes your website a lot more lively. But the question is, how does this work and how can you make this on your website?

It starts with using `transform`. The word says it all, this is to transform your element. You can use `perspective()` to create depth, `rotate()` to drive your website visitors crazy because they always have to turn their heads and use `translate()` to move your element around.

By using `perspective()` you give your element 3D space because you increase the space between the Z axis and the user. The smaller the value at perspective, the more intense the visual effect is.

Cool example from [Polypane](https://polypane.app/css-3d-transform-examples/) is this:
``` css
div {
  transform:
    rotateX(51deg)
    rotateZ(43deg);
  transform-style: preserve-3d;
  border-radius: 32px;
  box-shadow:
    1px 1px 0 1px #f9f9fb,
    -1px 0 28px 0 rgba(34, 33, 81, 0.01),
    28px 28px 28px 0 rgba(34, 33, 81, 0.25);
  transition:
    .4s ease-in-out transform,
    .4s ease-in-out box-shadow;

  &:hover {
    transform:
      translate3d(0px, -16px, 0px)
      rotateX(51deg)
      rotateZ(43deg);
    box-shadow:
      1px 1px 0 1px #f9f9fb,
      -1px 0 28px 0 rgba(34, 33, 81, 0.01),
      54px 54px 28px -10px rgba(34, 33, 81, 0.15);
  }
}
```
What comes out of that:

![image](https://user-images.githubusercontent.com/30145681/174489278-6658d3fe-f049-48bd-b270-491b6d524ef6.png)

This makes it look like the element is floating when you hover over it.

The options with 3D are almost endless and it also helps a lot with imitating real buttons or switches on websites for example. This way you can see even more clearly that, for example, you press a button or click a switch.

In short: 3D is cool, that's all I really need to say. It can improve the user experience and entertain people better on your website. It is also a nice challenge for yourself to make your website a bit 3D.

https://polypane.app/css-3d-transform-examples/

https://css-tricks.com/almanac/properties/p/perspective/

https://www.joshwcomeau.com/animation/3d-button/

https://www.sinds1971.nl/
