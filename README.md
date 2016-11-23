# foundation_newsletters
An attempt to improve our MXM newsletter workflow. You can use SASS and Foundation **WITHOUT ANY TABLES** :pray: to write proper tested email templates.
The buildsystem does all the ugly stuff for you. Comes with browsersync and more.

### Installation
1. If you need to build NEW newsletters for a project/client read on, to change a given project go to point 4.

2. Make sure foundation-cli is installed globally -> `npm install -g foundation-cli`

3. Navigate to the project folder and run -> `foundation new --framework emails`

4. Follow the instructions in the cli.

4. `npm install` and chill... it will take a few minutes to download and install all the stuff.

5.  To start the buildsystem with a server and all the watchers run -> `npm start`

### Production

All done? Run `npm run build` to merge and minify all the ugly tables and inline styles you need. Have fun :)

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
