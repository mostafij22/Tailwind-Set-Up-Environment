Step-1
=======
npm init --y
npm install -D tailwindcss
npx tailwindcss init

Step-2
=======
tailwind.config.js
------------------
    content: ["./*.html"],


Step-3
=======
input.css
---------
    @tailwind base;
    @tailwind components;
    @tailwind utilities;


Step-4
=======
npx tailwindcss -i ./input.css -o ./output.css --watch


Step-5
=======
package.json
------------
"scripts": {
    "dev": "tailwindcss -i ./input.css -o ./css/style.css --watch",
    "build": "tailwindcss -i ./input.css -o ./css/style.css"
},

Step-6
=======
Remove file: output.css 


Step-7
=======
Run command: npm run dev


Step-8
=======
index.html
-----------
Adding link in header: <link rel="stylesheet" href="./css/style.css">
