Setup Git 
---------
git init

git add .    // to add all the files

git commit -m "mesage"

git remote add origin [Origin URL from git]   // e.g. git remote add origin https://github.com/vinodwani18/NamasteReact.git

git push origin main

-------------------------------

Chapter notes:

Creating heading in html with javascript
----------------------------------------

cont heading =  document.createElement(heading);
heading.innerHTML = "heading 1"

cont root = document.getElementByID("root");

root.appendChild(heading);

--------------------------

Creating package configurations with NPM 
----------------------------------------
Use below command to configure your app using NPM 
:- npm init
It will ask basic stuff which needs to be entered.

-----------------------------------------

Bundlers available:
-----------
Webpack
Parcel
Vit

-------
Installing Parcel:
------------------
npm install -D parcel

Difference between ~ and ^ used in package.json with dependencies installed
--------------------------------
~ : Major versions can be upgraded if it gets released.
For ex. if we have depencency of parcel in our project and if a major version is released then it will automatically install it in project.

^ : Minor version can in upgraded.

--------------------------------

What is package.lock.json
----------------------
It keeps track of exact version installed in project whereas package.json keeps track of configuration used along with version provided with ^ or ~ .

-------------------------
Parcel:
-------
HMR - Hot module replacement : Parcel provides HMR properties to keep track of files changes by using file watcher algorithms.
Compression : Parcel provides compression properties to compress our files e.g images to optimize the performance of our app.
Minification : Parcel minifies the code.
Zero config : Unlike Webpack, Parcel requires zero configurations to setup.
Old browser competibility : Parcel allows support for older broser also.
Dev build 
local Server
Image optimaization
Bundling
Consistant hashing
Tree shaking : Parcel will remove unused code using tree shaing algorithm.

Install React and React.dom
-----------------------------
npm install react
npm install react-dom
npx parcel index.html
npx parcel build index.html
