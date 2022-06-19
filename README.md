# Weekly nerd

For the weekly nerd, every week a nerd comes to talk (surprise) about everything front-end. This is done by companies, former students, designers and professionals, often combinations of those!

## Learning goals
- Getting acquainted with the professional field
- Orientate on the field
- Learn to write subject-related articles

## Format of the readme:
[Articles](https://github.com/maggness/weekly-nerd-2122/README.md#articles)

[Weekly Nerd](https://github.com/maggness/weekly-nerd-2122/README.md#weekly-nerds)

[Weekly Mingle](https://github.com/maggness/weekly-nerd-2122/README.md#weekly-mingles)

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

## Article 3: Web Design & Dyslexia

There are many people who have dyslexia, I am one of them. We don't have the hardest time online, we can read but just not that good and fast. Not all dyslexics are the same, but there is an example website of what it looks like for some: http://geon.github.io/programming/2016/03/03/dsxyliea. How could you make a website more accessible for people with dyslexia?

There are a few basic points to keep in mind:
- use sans-serif fonts, these fonts are less crowded and easier to read with people who have dyslexia.
- You have to take larger fonts into account, some people with dyslexia make their fonts bigger because they can read better. Test your website carefully that everything is still in place if you make the text larger.
- Pay attention to word spacing, the bigger the font spacing, the easier the words are to tell apart. But make sure that the spacing is not too big, this makes it more difficult to read.
- Pay close attention to your headers, make them larger than the normal text so that it is easy to notice.
- The more text on an alina, the more difficult it is to read. Even if you have 2 columns next to each other with text.
- Uses BOLD instead of underlines, this is easier to read.

Many of these points are covered by general accessibility guidelines. It also helps to make your website very visual. Photos with items or using icons for things.

You should also pay close attention to contrast for texts. White on black or black on white is more difficult to read than, for example, black on beige. A dark gray font is also easier to read than a black font.

Many websites also have a search function that they depend on, this is really terrible for dyslexics. I myself have had many times where I couldn't find something because I could only search for it with text but only spelled it wrong.

It is not impossible to use most websites as a dyslexic, but it is super nice if the above points are taken into account.

https://www.succeedwithdyslexia.org/blog/creating-a-dyslexia-friendly-website-experience/#:~:text=The%20British%20Dyslexia%20Association%20recommends,Times%20New%20Roman%20and%20Georgia.

https://medium.com/branding101/designing-for-dyslexia-9e61945f82b0

https://uxplanet.org/designing-for-dyslexia-6d12e8c41cd7

http://geon.github.io/programming/2016/03/03/dsxyliea

# Weekly nerds

## Cyd Stumpel
<details>
<summary>Notes</summary>
Accessibility is more than important for a website.

You need to design your websites responsive so that every user can view your website

As a front-ender you need to be able to give advice on design and code.

Error states are very important to include when designing and creating your website. Also with forms
</details>

## Alvaro Montoro
<details>
<summary>Notes</summary>
All the way from Texas and has been in the business for over 15 years damn

You can also use CSS to draw, he makes art with CSS. Also css is good for reduced motion, responsiveness, user preferences & color contrast.

You can use 1 div's to make drawings

With clip path, masks, filters, blender mode, transformations, box-shadows & border radius you can make cool things.

https://alvaromontoro.com/projects (examples)
</details>

## Bram van Damme (CSS bonus)
 <details>
<summary>Notes</summary>
cascade is through can declarations determines which style you see

goes by priority, you have styling from the browser itself but they have less priority than your own. you have user preference, eg visually impaired > larger text. Transitions have the highest priority.

Newer css can @layer, works a bit like Photoshop with layers. First declared layer has the least priority and last highest priority. @layer layer name {}

@layer with the same name will be merged

at the top of your css file you can
`@layer name, name, name, name;`
this is how you declare the next of your layer

you can
`@import url(style.css)` to import other style
</details>
 
## Fenna de Wilde
  <details>
<summary>Notes</summary>
Websites need to be more accessible, unfortunately companies are not that busy with this yet. In America it is illegal to have an inaccessible website.

You don't necessarily have to put design aside to have a nice accessible website.

Think carefully about screen readers

In the future maybe let AI generate websites, now working on art.
</details>
  
## Nils Binder (Another CSS bonus)
<details>
<summary>Notes</summary>
<cite> for art

counter tag css, counter-increment & counter-reset

``` css
counter-reset:name;
counter-incement:name;

:before
content: counter(name, lower-alpha) ") ";
```

fancy border radius - github (useful)
 </details>
 
## Krijn Hoetmer
<details>
<summary>Notes</summary>
User friendly, and an extension of something physical, for example with buttons.

ask open feedback questions during an interview

A web app is never finished, you can always get feedback and improve it.

Keep it as simple as possible for users

Whatever you think of, it's being abused. even if you don't realize it: let people select wrong colors and then it will not be visible to the colorblind

Further development is difficult, if it becomes too complex it may no longer be accessible for some of your users. 
 </details>
 
 ## Vitaly Friedman
<details>
<summary>Notes</summary>

https://www.smashingmagazine.com/
https://yellowlab.tools/ (useful for testing)

some products are very complex, you have to make that easier for the users. Or make the complexity so that it works well for experts, such as at the dentist.

don't make navigation on your website too difficult, if it is very complex make it as structured as possible.

With complex nav good breadcrumbs.

No hover at menus > major irritation

no error messages under your form inputs, keyboard and everything gets in the way.

explanation of buttons that are disabled why they are
</details>
 
## Chanel Mepschen (Triple)
<details>
<summary>Notes</summary>
 
setup: Git, NPM, react/next.js & typescript

Typescript gives good feedback

eslint & prettier makes your code beautiful, clear

SASS > formulas in css, fewer errors

give customers preview

nice internship place?
 </details>
 
 ## Leonie Watson
<details>
<summary>Notes</summary>
 
You always start with the user architecture, not with graphic design but with voice design.

Screen readers can differ in voice, gender and, for example, accent. That's TTS, this tts keeps getting better and better

css speech module > not supported by most browsers

SSML > is used by google home etc

Give blind people the choice to skip content if they don't find it useful, makes alt texts longer with a nice and good description. More info = know what you can do with it / more atmosphere

make states clear when something is pressed, focus etc

Screen readers are not perfect, they often have things with pronunciation errors. You can't do anything about this
</details>

## Rian Rietveld
 <details>
<summary>Notes</summary>
  
Cognitive disabilities are, for example, people whose brains work differently

You have permanent cognitive limitations and temporary

Permanent is his e.g. ADHD, autism, dyslexia, anxiety disorder

Temporary: you are drunk or you have a hangover, sadness, angry, irritated, tired, noisy environment

Consistency navigation layout
- menu in the same place
- breadcrumbs on
- grip & clear title

Put names with icons, don't assume foreknowledge

With animations, make something calm. Give the user control whether they want to see the animation

No big pieces in all caps, that's hard to read

Use headings, subheadings & paragraphs

Make contacting as easy as possible, offer many options

Don't remove the label from forms when they fill in things, label above the input box
Put things that belong together
Tell what happens when you press the submit button
</details>
 
# Weekly Mingles
## Build in Amsterdam
Build in Amsterdam is a Digital agency that has large clients such as Adidas, Moooi, Mammut and Mollie. We went to the office and had a presentation by Folkert, he is an old CMDer. We also saw Carla, I talked to after a weekly nerd. He gave a short tour of the building and then he gave a presentation about Build in Amsterdam and working there.

As the first weekly mingle we didn't really know what to expect but it was super interesting. Nice to hear what our work might look like later and what your options are.

I got a good impression from the FOAM website they have been working on. This site was created during corona to mimic the museum online. The interaction and colors are very nice and less confessional.
 
## Label A
Week 2 we went to Label A, they are still at Leidseplein but will move in August. Then they will get a somewhat larger building because there are now so many people working there that there is no longer room for everyone. They also have an office in Rotterdam.

We had a short workshop and explanation about Typescript, which they use there. This is an extension to Javascript to give your code even more structure and to make it self-documented. They have some sort of academy for new hires to get them ready for work there. That way they are not just thrown in at the deep end.

For the workshop we got a github repo that we had to fork with 3 small assignments. First the base, then build on it. This was fun to do and more fun than just listening to a presentation.

 ## DEPT
Week 3 we went to DEPT. We got a tour of the office, which was a really nice. DEPT is already a large company with many offices, also abroad. They have shown cases that DEPT has worked on, such as one for the Haagsche Hogeschool. He also showed some code for this and how the templating works. DEPT also has a kind of academy for beginners/trainees.
 
## De Voorhoede
The last week we have been at De Voorhoede. After entering we had a small tour and we sat down for a presentation. During this presentation they talked about a project for Elsevier and how they have a big template where they input all the styling like colors to generate websites. They do this with components to ensure that large projects run smoothly.

We also made a kind of assignment, we had to circle the "Atoms", "Modules" and "Organism" and come up with good class names for this. The assignment was not clear enough at the moment so we accidentally made a breakdown sketch. After a little more explanation we knew better what “Atomic design” is.
