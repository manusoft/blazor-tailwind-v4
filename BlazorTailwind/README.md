
### Install Tailwind CSS
1. Install ```tailwindcss``` and ```@tailwindcss/cli``` via ```npm```.

```shell
npm install tailwindcss @tailwindcss/cli
```

### Import Tailwind in your CSS
2. Create a ```input.css``` file inside a ```Style``` folder of your project.

```css
@import "tailwindcss";
```

### Start the Tailwind CLI build process
3. Run the CLI tool to scan your source files for classes and build your CSS.

```shell
npx @tailwindcss/cli -i ./styles/input.css -o ./wwwroot/tailwind.css --watch
```

### Start using Tailwind in your HTML
4. Add your compiled CSS file to the <head> and start using Tailwind’s utility classes to style your content.

```html
<html>
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="tailwind.css" rel="stylesheet">
  </head>
  <body>
    <h1 class="text-3xl font-bold underline">
    Hello world!
    </h1>
  </body>
</html>
```