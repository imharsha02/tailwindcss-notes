# tailwind-css- notes

### Step 1:
Create a package.json file so that 'tailwindcss' can be installed. 

Now install tailwindcss using the command 'npm install tailwindcss'

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
