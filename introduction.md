# **LESS**

* Extention of CSS & dynamic style sheet language.
* CSS pre-processor.
* It provides @import rule.

## **CSS Preprocessor**

* Extention of CSS & read by web browser.
* It provides variables,functions,mixins & opreations etc.
* LESS & SASS both are ex of CSS.

## **Less Installation**

1. **OS   **                       ** :**cross\_platform
2. **Browser support:**IE,Firefox,Google chrome,Safari

To install Node.js  on windows to the link [https://nodejs.org/en/](https://nodejs.org/en/)

Download current version & install less on server via NPM\(Node Package Manager\)

```
"npm install -g less" -->into cmd prompt
```

#### **Less Example**

Create html file "Sample.html"

```
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="sample.css" type="text/css"/>
</head>
<body>
<h2>less ex</h2>
<h3>css</h3>
</body>
</html>
```

Create less file "sample.less"

```
@primarycolor:#ffffff;
@color:#800080;
h2{
color:@primarycolor;
}
h3{
color:@color;
}
```

Both file sample.html & sample.less inside the root folder of Node.js

Go to cmd[^1] prompt

```
-->npm install -g less
-->cd desktop
-->lessc sample.less sample.css
```

To compile sample.less & CSS file will be  generated named at sample.css.

Generated CSS "sample.css"

```
h2{
color:#ffffff;
}
h3{
color:#800080;
}
```

Output will be generated.

## **Less Comments**

1. Singleline comment://don't display in CSS o/p.
2. Multiline comment  :/\*?.\*/preserved in generated CSS o/p.

For ex to refer this link[ https://www.javatpoint.com/less-comments](https://www.javatpoint.com/less-comments)

#### **Less Syntax**

It is non-standard as per W3C specification.

#### **Less code:**

```
@color-base:#2d5e8b;
.class1{
background-color:@color-base;
.calss2{
background-color:#fff;
color:@color-base;
}
}
```

#### **CSS code:**

```
.class1{
background-color:#2d5e8b;
}
.class2{
background-color:#fff;
color:#2d5e8b;
}
```

## **Less Variables**

* It's defined with a symbol @
* And values are assign in the variable with colon\(:\)

For ex to refer this link [https://www.javatpoint.com/less-variables](https://www.javatpoint.com/less-variables)

## **Less Variable Scope**

* It's specifies a place of available variable.
* 1st the variable search from local scope, there is not available then they search parent scope by compiler.

For ex to refer this link [https://www.javatpoint.com/less-variable-scope](https://www.javatpoint.com/less-variable-scope)

## **Less Extend**

* It is a feature of less.
* It acts as using : extend selector.

For ex to refer this link [https://www.javatpoint.com/less-extend](https://www.javatpoint.com/less-extend)

## **Less Nesting**

* The code follow some visual hierarchy.
* It makes your code simple,clean,less complex.

For ex to refer this link [https://www.javatpoint.com/less-nesting](https://www.javatpoint.com/less-nesting)

## **Less Importing**

Less depending on the file extention by using @import statements.

For ex to refer this link [https://www.javatpoint.com/less-importing](https://www.javatpoint.com/less-importing)

## **Less Import Options**

* More than one keyword in @import statement.
* To seperate those keyword by comma.

For more details to refer this link [https://www.javatpoint.com/less-import-options](https://www.javatpoint.com/less-import-options)

#### **for ex:**

```
@import(less,optional)"sample.css"
```

## **Less Operations**

* It supports some arithmetic operations llike addition\(+\),subraction\(-\),multiplication\(\*\) & division\(/\).
* It can be done on any number,color & variable.

For ex to refer to this link [https://www.javatpoint.com/less-operations](https://www.javatpoint.com/less-operations)

## **Less Mixins**

* To add bunch of ppy[^2] from one rule-set into another rule-set.
* It's a CSS style using class or id selector.
* It can store multiple values.

For ex to refer this link [https://www.javatpoint.com/less-mixins](https://www.javatpoint.com/less-mixins)

### 1.**Less Parametric Mixins**

```
.border(@width;@style;@color){
border:@width@style@color;
}
.myheader{
.border(5px;dashed;red)
}
```

### 2.**Less Mixins as Functions**

To refer this lilnk [https://www.javatpoint.com/less-mixins-as-functions](https://www.javatpoint.com/less-mixins-as-functions)

### 3.Passing Rulesets to Mixins

To refer this link [https://www.javatpoint.com/less-passing-ruleset-to-mixin](https://www.javatpoint.com/less-passing-ruleset-to-mixin)

## **Less Loops**

* To execute a statement or group of statements multiple times.

For ex to refer this link [https://www.javatpoint.com/less-loops](https://www.javatpoint.com/less-loops)

## **Less Merge**

To aggerate valuse from multiple ppy into a comma or space.

#### **Types**

1. **Comma** -Used to add ppy value to end.
2. **Space** - Used to ppy value with space.

### 1.**Less Merge Comma**

To refer this link [https://www.javatpoint.com/less-merge-comma](https://www.javatpoint.com/less-merge-comma)

### 2.**Less Merge Space**

To refer this link [https://www.javatpoint.com/less-merge-spaceLess Merge Space](https://www.javatpoint.com/less-merge-spaceLess Merge Space)

## **Less Parent Selectors**

They are denoted by &\(ampersand\) operator.

#### **Types**

1. Multiple &                             -The & represent nearest selector and also all parent selector.
2. Changing Selector Order -The inherited\(parent\) selectors is usefull.
3. Combinatorial Explotion  -The selectors in the  list are  separated by comma.

For ex to refer this link [https://www.javatpoint.com/less-parent-selectors](https://www.javatpoint.com/less-parent-selectors)

### 1.**Less MP Selector\(Multiple & Parent Selector\)**

To refer this link [https://www.javatpoint.com/less-multiple-and-parent-selector](https://www.javatpoint.com/less-multiple-and-parent-selector)

### 2.**Less CSOP Selector\(Changing Selector Order Parent Selector\)**

To refer this link [https://www.javatpoint.com/less-changing-selector-order-parent-selector](https://www.javatpoint.com/less-changing-selector-order-parent-selector)

### 3.**Less CEP Selector\(Combinatorial Explosion Parent Selectors\)**

To refer this link [https://www.javatpoint.com/less-combinatorial-explosion-parent-selectors](https://www.javatpoint.com/less-combinatorial-explosion-parent-selectors)

## **Less Functions**

* A lot of functions such as  round function,floor function,cell function,percentage function etc.
* Less to manipulate colors & HTML elements aspects in style sheets.

For ex to refer this link [https://www.javatpoint.com/less-functions](https://www.javatpoint.com/less-functions)

## **Misc Functions**

A group of functions of different types.

1.**Less color\(\)** -Used to represent colors.

To refer this link [https://www.javatpoint.com/less-color-function](https://www.javatpoint.com/less-color-function)

2.**Less image-size\(\)** -Check dimension of the image.

To refer this link [https://www.javatpoint.com/less-image-size-function](https://www.javatpoint.com/less-image-size-function)

3.**Less image-width\(\) **-Check width of the image.

To refer this link [https://www.javatpoint.com/less-image-width-function](https://www.javatpoint.com/less-image-width-function)

4.**Less image-height\(\)** -Check height o hte image.

To refer this link [https://www.javatpoint.com/less-image-height-function](https://www.javatpoint.com/less-image-height-function)

5.**Less convert\(\)** -Convert no from one unit to another.

To refer this link [https://www.javatpoint.com/less-convert-function](https://www.javatpoint.com/less-convert-function)

6.**Less data-url\(\)** -Uniform resource identifier resource in web pages.

To refer this link [https://www.javatpoint.com/less-data-uri-function](https://www.javatpoint.com/less-data-uri-function)

7.**Less default\(\)** -It returns true only.

To refer this link [https://www.javatpoint.com/less-default-function](https://www.javatpoint.com/less-default-function)

8.**Less unit\(\)** -It returns ture only.

To refer this link [https://www.javatpoint.com/less-unit-function](https://www.javatpoint.com/less-unit-function)

## **Less List Functions**

To specify length of the list & position of value in the list.

#### **Types**

1. **Length** -A comma or space separated list of values as parameter.
2. **Extract -**Return the value at specified position in a list.

### 1.**Less List Length\(\)**

To refer this link [https://www.javatpoint.com/less-list-length-function](https://www.javatpoint.com/less-list-length-function)

### 2.**Less List Extract\(\)**

To refer this link [https://www.javatpoint.com/less-list-extract-function](https://www.javatpoint.com/less-list-extract-function)

## **Less Math Functions**

* Used to perform numeric operations such as round,square root,power value,modulus,percentage etc.

To refer this link [https://www.javatpoint.com/less-math-functions](https://www.javatpoint.com/less-math-functions)

## **Less Type Functions**

* Used to determine the type of the value.

To refer this link [https://www.javatpoint.com/less-type-functions](https://www.javatpoint.com/less-type-functions)

### **Less Color Definition Functions**

* To alternate & manipulate colors in different ways.

To refer this link [https://www.javatpoint.com/less-color-definition-functions](https://www.javatpoint.com/less-color-definition-functions)

### **Less Color Channel Functions**

* There are built-in functions which are  used to set value about a channel.

To refer this link [https://www.javatpoint.com/less-color-channel-functions](https://www.javatpoint.com/less-color-channel-functions)

### **Less Color Operation Functions**

* To alter & manipulate colors in different ways.

To refer this link [https://www.javatpoint.com/less-color-operation-functions](https://www.javatpoint.com/less-color-operation-functions)

### **Less Color Blending Functions**

* Used in image editors like Photoshop,Fireworks or GIMP.

To refer this link [https://www.javatpoint.com/less-color-blending-functions](https://www.javatpoint.com/less-color-blending-functions)

---
