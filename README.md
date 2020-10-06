# tailwind-css- notes

### Step 1:
Create a package.json file so that 'tailwindcss' can be in

Now install tailwindcss using the command
```html
npm install tailwindcss
```

### Step 2:
Inside the project folder, create two sub-folders called 'src' and 'public'

### Step 3:
Inside the src folder, create a styles.css.
Inside the styles.css, past the following lines of code:
```html
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### Step 4:
Inside the script tags of the package.json file, paste the follwoing script
```html
 "build-css":"tailwindcss build src/styles.css -o public/styles.css"
```

### Step 5:
Now run the script in the terminal using the following command:
```html
npm run build-css
```
### Step 6:
Inside the public folder, along with styles.css (which will be present), create a html file.

### Step 7:
Now all that is to add tailwindcss classes for styling


### Modify font size
The way to write a class to change font size is
```html
font-size(integer or integerAlongWith)
```
### Text colors
The way to write a class to change the font color is 
```html
text-color-darkOrLight(number)
```
### Background-color
The way to set background color is:
```html
bg-colorName-strength
```
Not only solid colors, but transperentness can be set using
```html
bg-transparent
```

### Font style
```html
font-styleName
```

### Margin
```html
m-amountOfMargin
```
This adds margin all around the content present inside the tag to which this class was applied

### Margin one-side
```html
mt-amountOfMargin
```
Adds a top margin.
Similarly, mb, mr and ml classes can be applied to provide margins to the bottom, right and left side of the content

### padding to all sides
```html
p-amountOfPadding
```
### Horizontal padding
```html
px-amountOfPadding(number)
```
### Vertical padding
```html
py-amountOfPadding(number)
```

### Customizing styles
To customize styles, a tailwind config file is need.
The file is created using:
```html
npx tailwindcss init
```
Using the cofig file, new properties can be added or properties that are present can be removed or modified.
The properties must be added in the 'extend' object so that the default tailwindcss properties can be accessed or modified.
After modifing the config file, the website must be built again using the command:

```html
npm run build-css
```

After building, the costum color can be used by adding the following class:

```html
bg-<cosutumColor>-strength
```

There are few points to be noted here:
1) The signatures of the default config file and the custom config file must be the same. So, it is better to take the default config file as refrence.
2) Each and every time the custom file is modified, the website must be rebuilt

### Custom fonts
To use custom fonts, first that font needs to be imported into the syles.css file in the src folder.
Now inside the config file, we can add a new property to the fontFamily object. The name of the property can be anything, but the value must be an array.
Now since it is imported into the styles.css file, no error will be produced.

To use the custom font, use the class
```html
font-<nameOfTheProperty>
 ```
 
 ### Flexbox and tailwindcss
 
 To display something in flex, use the class:
 ```html
flex
```
All the properties of flex can be used.
For example, the class 'justify-center' centers the content horizontally.However, since justify-center ultimately uses 'justify-content:center' which is related to flex, it must be used alongside the flex class
 
### Width and height in tailwind
To add width and height, use the class

```html
h-<verticalLengthInNumbers> for height and w-<AmountOfWidthInNUmbers>
 ```

### Align items vertically
Use the class 
```html
items-<position>
 ```
 alongside the flex class to align items vertically


























