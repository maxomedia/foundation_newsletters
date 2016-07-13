# foundation_newsletters
An attempt to improve our newsletter workflow. You can use SASS and Foundation WITHOUT ANY TABLES to write proper tested email templates.
The buildsystem does all the ugly stuff for you. Comes with browsersync and more.

### Installation
1. Clone the develop branch of this repo.

2. If you would like to build newsletters for a new project/client read on,
	 otherwise, if you need to change something or build newsletters for an existing project, go to point 5.

2. If you would like to build newsletters for a new project/client -> `npm install -g foundation-cli`
3. Name the project like "Maxomedia Newsletters", "SBB" or what ever.
4. Take a coffee, it will take a few minutes to download all the stuff...

5. Navigate to the subfolder of the project and run `npm start` - this will start the buildsystem with a server and all the watchers.

### File Structure

Here's a breakdown of the files in the src folder:
`assets/` 	: Sass and image files.
`layouts`		: Boilerplate HTML that wraps all of your emails.
`partials/` : Reusable chunks of HTML that can be injected into pages.
`pages/` 		: HTML files for emails.

Everything runs through the buildsystem and you'll find the final newsletter html in the `dist` folder.

### Handling
Foundation for Emails includes many common elements needed to make HTML emails: a grid, typography styles, buttons, callouts, and more.
Basically it's almost the same like Bootstrap, just some classnames are different.

There's also a `default.html` - this is needed to create the table layout in the end. ####Just don't remove it!####

Further informations how to write it: [foundation documentation] (http://foundation.zurb.com/emails/docs/sass-guide.html)

### Production

All done? Then run `npm run build` and it will generate all the ugly tables and inline styles you need. All minified in one line.
Have fun :)
