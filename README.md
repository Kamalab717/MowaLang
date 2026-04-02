<h1 align="center">MOWALANG</h1>
<p align="center">
<a href="https://lgtm.com/projects/g/DulLabs/bhai-lang/alerts/"><img alt="Total alerts" src="https://img.shields.io/lgtm/alerts/g/DulLabs/bhai-lang.svg?logo=lgtm&logoWidth=18"/></a>
<a href="https://lgtm.com/projects/g/DulLabs/bhai-lang/context:javascript"><img alt="Language grade: JavaScript" src="https://img.shields.io/lgtm/grade/javascript/g/DulLabs/bhai-lang.svg?logo=lgtm&logoWidth=18"/></a>
<a href="https://github.com/DulLabs/bhai-lang/actions/workflows/node.js.yml/badge.svg"><img alt="Build" src="https://github.com/DulLabs/bhai-lang/actions/workflows/node.js.yml/badge.svg"/></a>
<a href="https://mowalang.js.org/"><img alt="Build" src="https://img.shields.io/badge/website-mowalang.js.org-orange"/></a>
<a href="https://www.npmjs.com/package/mowalang"><img alt="Build" src="https://img.shields.io/badge/npm-mowalang-orange"/></a>
  
</p>
<p align="center">
  This is official repository for MOWALANG.<br><br>
  <b>MOWALANG is a toy programming language written in Typescript.</b>
</p>
<br>

<h2 align="center">Installation</h2>

```
npm i -g mowalang
```

<h2 align="center">Usage</h2>

<h4 align="left">Create a new file (<code>test.bhai</code>)</h4>


<h4 align="left">Edit the file with a text editor.
You can also try out your code on <a href="https://mowalang.js.org/#playground">MOWALANG PlayGround</a></h4>

```
hi mowa
  cheppu ra mowa "Hello mowa";
bye mowa

```

<h4 align="left">Run</h4>

```
mowalang test.bhai
```

<h4 align="left">Output</h4>

```
hello mowa
```

<h2 align="center">Documentation</h2>

<h3 align="center">General</h3>
<p align="center"><code>hi mowa</code> is the entrypoint for the program and all program must end with <code>bye mowa</code>. Anything outside of it will be ignored.</p>

```

This will be ignored

hi mowa
// Write code here
bye mowa

This too
```

<h3 align="center">Variables</h3>
<p align="center">Variables can be declared using <code>mowa idhigo ra</code>.</p>

```

hi mowa
  mowa idhigo ra a = 10;
  mowa idhigo ra b = "two";
  mowa idhigo ra c = 15;
  a = a + 1;
  b = 21;
  c *= 2;
bye mowa
```

<h3 align="center">Types</h3>
<p align="center">Numbers and strings are like other languages. Null values can be denoted using <code>em ledhu dolla</code>. <code>saripoindhi mowaaa</code> and <code>thapppu ra mowa</code> are the boolean values.</p>

```

hi mowa
  mowa idhigo ra a = 10;
  mowa idhigo ra b = 10 + (15*20);
  mowa idhigo ra c = "two";
  mowa idhigo ra d = 'ok';
  mowa idhigo ra e = em ledhu dolla;
  mowa idhigo ra f = saripoindhi mowaaa;
  mowa idhigo ra g = thapppu ra mowa;
bye mowa
```

<h3 align="center">Built-ins</h3>
<p align="center">Use <code>cheppu ra mowa</code> to print anything to console.</p>

```

hi mowa
  cheppu ra mowa "Hello World";
  mowa idhigo ra a = 10;
  {
    mowa idhigo ra b = 20;
    cheppu ra mowa a + b;
  }
  cheppu ra mowa 5, 'ok', em ledhu dolla , saripoindhi mowaaa , thapppu ra mowa;
bye mowa
```

<h3 align="center">Conditionals</h3>
<p align="center">MOWALANG supports if-else-if ladder construct , <code>mowa idhi aythe</code> block will execute if condition is <code>saripoindhi mowaaa</code>, otherwise one of the subsequently added <code>mowa idhi kaakapothe</code> blocks will execute if their respective condition is <code>saripoindhi mowaaa</code>, and the <code>idhi kuda kaakapothe</code> block will eventually execute if all of the above conditions are <code>thapppu ra mowa</code>

```

hi mowa
  mowa idhigo ra a = 10;
  mowa idhi aythe (a < 20) {
    cheppu ra mowa "a is less than 20";
  } mowa idhi kaakapothe ( a < 25 ) {
    cheppu ra mowa "a is less than 25";
  } idhi kuda kaakapothe {
    cheppu ra mowa "a is greater than or equal to 25";
  }
bye mowa
```

<h3 align="center">Loops</h3>
<p align="center">Statements inside <code>mowa idhi ayye dhaaka</code> blocks are executed as long as a specified condition evaluates to saripoindhi mowaaa. If the condition becomes <code>thapppu ra mowa</code>, statement within the loop stops executing and control passes to the statement following the loop. Use <code>aapey ra mowa</code> to break the loop and <code className="language-cpp">inkoti choodu mowa</code> to continue within loop.</p>


```

hi mowa
  mowa idhigo ra a = 0;
  mowa idhi ayye dhaaka (a < 10) {
   a += 1;
   mowa idhi aythe (a == 5) {
    cheppu ra mowa "andar se cheppu ra mowa ", a;
    inkoti choodu mowa;
   }
   mowa idhi aythe (a == 6) {
    aapey ra mowa;
   }
   cheppu ra mowa a;
  }
  cheppu ra mowa "done";
bye mowa
```

<h2 align="center">Development</h2>
<p align="center">You can explore abstract syntax tree(AST) of mowalang <a href="https://mowalang-ast.netlify.app/" target="_blank">here</a>.</p>








