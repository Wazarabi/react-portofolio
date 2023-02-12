## HOW WE CREATED THIS :
0. Vocabulary
    1. Create ( file, folder ...)
    2. Add ( fct, class, script ...)
    3. COPY ( file, fct ...)
    3. Run ( cmd in terminal )

1. Install dev tools
    1. VS CODE EXTENSION : Tailwind CSS IntelliSense

2. Init / Scaffolding the project
    1. RUN *npx create-next-app@latest app-name*
    2. RUN *npm install -D tailwindcss*
    3. RUN  *npm install -D tailwindcss postcss autoprefixer* && *npx tailwindcss init -p*
    >> CREATES tailwind.config.js && postcss.config.js
    4. COPY **/public** folder from GITHUB : *https://github.com/developedbyed/react-portofolio-with-tailwind* (contains the assets)
    5. RUN *npm run dev*
    6. CLEAN APP FILE : **pages/index.js** -> Keep the *Head* & an empty *main*
    7. MODIFY *styles/globals.css*
        1. CLEAN CSS FILE : **styles/globals.css** -> COPY STARTER CODE FROM SAME *GITHUB*
        2. ADD the classes and utilities at the top of **styles/globals.css** FILE ->
        *@tailwind base; @tailwind components; @tailind utilities;*
        3. ADD the BURTON *font* to the bottom of **styles/globals.css** FILE ->
        *@font-face{*
            *font-family:"burtons";*
            *src:url("../public/Burtons.otf");*
        *}*
    8. VS Code Tailwind Extension
        1. INSTALL EXTENSION : *Tailwind CSS IntelliSense* >> TO get AutoCompletion & Linting
        2. MODIFY VS CODE SETTINGS in *settings.json* >> OPEN FILE through *>Preferences: Open Settings (JSON)* command
        **"editor.quickSuggestions": {**
            **"other":"on",**
            **"comments":"off",**
            **"strings": "on"**
        **},**
        **"files.associations": {**
            **"*.css": "\"tailwindcss\""**
        **}***
    9. RUN *npm i react-icons*
    10. COPY config for template paths from Tailwind docs 2 **tailwind.config.js**
    11. Test that TailwindCSS is functionnal (add tailwind classes to something and see if it workds)