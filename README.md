
# CSS MOSTLY USED CLASS GENERATOR BY USING SCSS

I created this project to get my work done quickly. Those who work as frontend developers know that SCSS is essential for completing projects quickly.

I have tried to show in this small project how easily we can use css classes in our daily projects like margin-top, padding-top, margin-bottom, padding-bottom, z-index, postion-helper class, flex-box , postion class, font-weight, height, width, text-alignment, border-radius etc. 

The classes are shown so that we can create the class as per our project requirements just once without writing the style again and again. Although many people may know this. Those who don't know or need to copy and paste the same CSS code for each project, I hope it will be useful for them.


## Installation

Clone from github:

```bash
  git clone https://github.com/webcoder97/css-generator-by-scss.git
  cd css-generator-by-scss
```
npm install:
```bash
  npm init
```
Install Sass Compiler:
```
npm install node-sass --sass-dev
```

Run Compiler for dev mode:
```bash
  npm run dev
```

Run Compiler for production mode:
```bash
  npm run build
```

<!-- ## Screenshots

Unminfied CSS (dev Mode)

![App Screenshot](https://i.ibb.co/1RvRfhw/code-unminify.png)

Minified CSS (Production Mode)

![App Screenshot](https://i.ibb.co/YtBxX4M/minfiy.png) -->


## Usages
For margin use class = mt-$value
Please Remember: $value increasing start from 5 to 30, 
This means you can use last class = mt-150 and same as mr-$value, ml-$value, mb-$value,
Please Note: mt= margin-top, mb= margin-bottom, mr= margin-right, ml= margin-left;

```html
<!-- for margin -->
<div class="mt-0">
  <p>you can use mt, mb, ml and mr classes, just write ml-50 for margin-left: 50px;</p>
</div>

<!-- for padding -->
<div class="pt-0">
  <p>you can use pt, pb, pl and pr classes, just write pl-50 for padding-left: 50px;</p>
</div>
```
if you need value more than 150, you can change easily
```scss
@for $i from 0 through 30 {
	$remValue: ($i * 5) / $baseFont;
	.mt-#{$i * 5} {
	  margin-top: #{$remValue}rem;
	}
}
```
Just change value '30' to as your need.


## Authors

- [@Md. Saiful](https://github.com/webcoder97)

