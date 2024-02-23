# kattos-jatek

0.git clone
1.terminal bash->npm init -y
2.delete the main line from pacakge.json
3.npm i parcel
4.npm i gh-pages
5.npm i rimraf
6.new section dependencies ->compare/overwrite
7.insert:
"build": "rimraf dist && parcel build './src/**/*.html' --no-cache",
"start": "rimraf dist && parcel serve './src/**/*.html' --no-cache --open",
"deploy": "gh-pages -d dist"

in between scripts bracket
8.create .gitignore
9.write node_modules and dist in it
10.create new folder -src
11.create index.html
12.create scripts and styles folder
13.html: div id reslut, div id box
14.create link rel in html /src/styles
15.script src=/src/scripts/index.js
16.create index.js file
17.changed build start in package json to this:
"build": "rimraf ./dist && parcel build ./src/index.html --no-cache --dist-dir ./dist",
    "start": "rimraf ./dist && parcel serve ./src/index.html --no-cache --open",
    18.gitignore .parcel-cache