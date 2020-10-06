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
To add vertical padding, use
```html
py-amountOfPadding(number)
```
































