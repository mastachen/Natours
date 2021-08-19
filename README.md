# Natours
 First project of advanced css course

BEM (block element modifier)
	.block (standalone component, meaningful on its own)
	.block__element (part of a block with no standalone meaning)
	.block__element--modifier (a different version of a block or an element)
	
7-1 CSS architecture

Creating package.json
	- Npm init

Install sass locally (as a dev dependency)
	- Npm install node-sass --save-dev

Automatic compiling of sass 
	- Define script in package.json
	{
	  "name": "natours",
	  "version": "1.0.0",
	  "description": "Landing page for natours",
	  "main": "index.js",
	  "scripts": {
	    "compile:sass": "node-sass sass/main.scss css/style.css -w"
	  },
	  "author": "Primi",
	  "license": "ISC",
	  "dependencies": {},
	  "devDependencies": {
	    "node-sass": "^4.14.1"
	  }
	}
	- Run it with command: npm run compile:sass
	- -w stands for watch (generate css file when change is detected)
	- Must run in separate terminal all the time

Automatic reload
	- Live server install
		○ Npm install live-server -g
	- Run it with command: live-server

Npm install concat save--dev
Npm install autoprefixer --save-dev
Npm install postcss-cli --save-dev![image](https://user-images.githubusercontent.com/9267684/130050970-bb4b26df-bf3f-4481-869c-57c825765c5f.png)
