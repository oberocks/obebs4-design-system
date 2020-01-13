# OBE:BS4 Design System

The OBE:BS4 Web Design System is the world's first self-reflexive web design system for web production. OBE:BS4 is based on the most popular/robust front-end web framework in the world, Bootstrap! The OBE:BS4 system was designed & built to give all project stakeholders complete visual & tactile access to every color, font, element, component, & layout in a web project... *before the project enters any design phases!*

THE OBE:BS4 Web Design System was designed to bridge the gaps between web project owners, designers, and developers. OBE:BS4 achieves this goal by fostering a more healthy understanding of both code and design *constraints* in the context of the final output medium(s)... the web browsers!

> **Please Note:** *This project is fully functional as far as the generated CSS, JS, and library HTML files are concerned. However the code will receive _substantial changes_ before being ready for all to use. Please consider this an alpha version, and keep an eye on this page to learn more about how everything works as documentation is figured out. Once the project is rezady, an offical release will follow!*


---


## Table of Contents

* [About The Project](#about-the-project)
* [Project Color Wheel](#project-color-wheel)
    * [List of Color Wheel Colors](#list-of-color-wheel-colors)
    * [Examples of Color Tints and Shades](#examples-of-color-tints-and-shades)
    * [The Color Codes Table](#the-color-codes-table)
    * [Accessing Colors with JavaScript](#accessing-colors-with-javascript)
* [Project Workflow](#project-workflow)
    * [Project Directories](#project-directories)
    * [Project Build Tooling](#project-build-tooling)
* [Installation](#installation)
    * [Installing via NPM](#installing-via-npm)
* [Updating Versions](#updating-versions)
    * [Updating OBE:BS4 to Latest Version](#updating-obebs4-to-latest-version)
    * [Updating OBE:BS4 Build Scripts for Gulp](#updating-obebs4-build-scripts-for-gulp)
    * [Updating OBE:BS4 obebs4_settings.json file](#updating-obebs4-obebs4settingsjson-file)
* [Customizing Your Library](#cutromizing-your-library)
    * [Bringing System Directories to Root](#bringing-system-directories-to-root)
    * [Adjusting the Gulp File](#adjusting-the-gulp-file)
    * [Library Site Files](#library-site-files)
* [Roadmap](#roadmap)

<!--- * [Installing via Zip](#installing-via-zip) -->

---


## About The Project

The OBE:BS4 Web Design System is meant to nudge web projects, web teams, and even entire web organizations towards making both strategic & design related decisions about their projects *exclusively within* the contexts of the browsers. This approach has tremendous value, especially when seeking a high-caliber device agnostic web user experiences.

OBE:BS4 doesn't assume designers are incapable of learning how to hack a little markup or throw around some HTML snippets. Instead, the OBE:BS4 web design system arms designers with both visual and markup examples of anything/everything a designer might need to solve a web-based design problem.

> *"OBE:BS4 assumes that everyone working on a web project needs transparent access to each option and each limitation for the client-facing side of the project at all times."* - Matt McT

Accomplishing this is done through a surprisingly simple operational tweak. The secret is creating a work flow where the front-end specialists are expected to give the design specialists a complete reference of all available design options provided by both browsers and any applicable libraries/frameworks.

Here's the catch though, and why this isn't happening all over the world today... all of this needs to happen **_before_** any design work begins!!! Designers need to see/touch whatever is available for use in designs, and also see/touch differences across browsers **_before_** they start thinking about how to best solve problems! The only way to do that though... would be to make a customizable website that displays... everything!? Who got time (or money) for dat???

Enter OBE:BS4! ;)

Additionally, what's magical about this situation from a developer's POV, is how it gives front-end specialists an opportunity to refactor and templatize elements/components at a production level, before **_any_** design sprints begin. This allows engineers to create amazingly DRY markup templates/scripts, and to engineer solutions the "right" way from the get-go according to the tech stack.

> *"The aspect of this project that excites me the most, is how much further a team's strategic thinking and prototyping can reach upon embracing the OBE:BS4 process. It becomes clear after using the system fully, that somehow we've all accidentily been doing this web stuff in the wrong order all these years! D'OH!"* - Matt McT

The OBE:BS4 Web Design System positions **_all_** project stakeholders to think more strategically about *responsive* content issues, by abstracting the design options to proactively to solve those issues into a tangible digital "toolbox" of fully responsive and designer-ready pieces.

If each piece is in-turn *proactively* optimized for production (IE valid, semantic, cross-browser, ARIA accessibile, and refactored for reuse), teams find themselves with an abundance of cognative room to focus on the more meta-level goals of any given web project.

<!---
You know, stuff like:
1. Device Agnostic Designs
1. Improving Content Consumption
1. Increasing eCommerce Conversions
1. 508 Compliance
1. Device Agnostic & Accessible SaaS Services
1. Ensuring Projects Are Maintainable/Reusable (For Devs)
-->

---


## Project Color Wheel

To work with the OBE:BS4 Web Design System, it's important to understand the system's "color wheel." Before we dive in, let's cover why a color wheel was necessary to begin with!

Long story short, it started with the Bootstrap "contextual" color classes (primary, danger, etc.) which were combined with Google's Material Design color guidelines. Next, branding was factored in, including concerns for both digital and analog collateral design needs. To organize all of that complexity into a customizable solution, and to ensure contingency color options for both digital and analog design edge cases, the color wheel system emerged!

The color wheel itself is used to integrate any current branding into the OBE:BS4 build system. Then by using the system's built-in settings tool (Example: [OBE:BS4 Settings Page](https://library.mattmct.com/settings.html)), you can specify your settings, grab the generated JSON, replace your existing settings file with your new JSON data, and finally re-generate your library site (HTML, CSS, & JS files) with your new settings!

### List of Color Wheel Colors

PRO TIP: If possible, try to memorize these slugs and patterns! Knowing these will let you iterate VERY rapidly!

| Name | CSS Slug | JS Slug |
| --- | --- | --- |
| Red | red | red |
| Rose | rose | rose |
| Magenta | magenta | magenta |
| Violet | violet | violet |
| Blue | blue | blue |
| Azure | azure | azure |
| Cyan | cyan | cyan |
| Spring Green | spring-green | springGreen |
| Green | green | green |
| Chartreuse | chartreuse | chartreuse |
| Yellow | yellow | yellow |
| Orange | orange | orange |
| Orange Gray | orange-gray | orangeGray |
| Dark Gray Orange | dark-gray-orange | darkGrayOrange |
| Blue Gray | blue-gray | blueGray |
| Light Gray Azure | light-gray-azure | lightGrayAzure |
| White | white | white |
| Light Gray | light-gray | lightGray |
| Gray | gray | gray |
| Dark Gray | dark-gray | darkGray |
| Black | black | black |

### Examples of Color Tints and Shades

PRO TIP: When using the Web Design System's tints and shades, each color gets a set of tint and shade values like the example for Blue below. Also for all color options with tints and shade classes, using the color slug without any numbers is equal to the 500 variation of that color. So for example, "Blue" is equal to "Blue 500", "White" to "White 500", and so on!

| Name | CSS Slug | JS Slug |
| --- | --- | --- |
| Blue 50 | blue-50 | blue50 |
| Blue 100 | blue-100 | blue100 |
| Blue 200 | blue-200 | blue200 |
| Blue 300 | blue-300 | blue300 |
| Blue 400 | blue-400 | blue400 |
| Blue | blue | blue |
| Blue 500 | blue-500 | blue500 |
| Blue 600 | blue-600 | blue600 |
| Blue 700 | blue-700 | blue700 |
| Blue 800 | blue-800 | blue800 |
| Blue 900 | blue-900 | blue900 |

### The Color Codes Table

The OBE:BS4 web design system allows you to centralize your brand colors for web projects. It can also be used for non-web design disciplines, too. OBE:BS4 makes the challenge of keeping brand colors consistent across projects/mediums trivial.

If you host your library, Visual Designers can use the web design system's client-side generated [Color Reference Table](https://library.mattmct.com/reference.html#color-codes-table) to quickly find color codes for each color in the system. This means that it takes only seconds to add exact colors (even recently updated colors ;) into Photoshop, Illustrator, PowerPoint, Social Network account settings, video work, and so much more.

The Color Codes Table is basically the best tool your team never knew they needed.

### Accessing Colors with JavaScript

The Color Codes Table is great for designers and marketers and all... but what about when those color codes are needed in JavaScript???

That's exactly what the client-side generated [JavaScript/JSON Snippets](https://library.mattmct.com/reference.html#accessing-obebs4-colors-javascript) part of the system is for!

A developer can simply parse the generated JSON strings, and access the color codes using the JS Slugs conventions in the table above.

For example, you could to make a seperate JavaScript file, and parse your colors JSON string as you assign it to a variable. Then you can include/require it on pages/components as needed. Here's a super simplified way to demonstrate how to use OBE:BS4 color wheel colors in JavaScript:

```javascript
// EXAMPLE: An external .js file named brandColors.js
const brandColors = JSON.parse('PASTE_RGBa_JSON_INSIDE_THESE_QUOTES');
```

```javascript
// EXAMPLE: Utility function to customize the alpha value of an rgba string
// NOTE: The Default alpha value for all RGBa strings is: '0.5'
const setRGBa = function (rgbaString, alphaValue) {
    return alphaValue ? rgbaString.replace('0.5', alphaValue) : rgbaString;
}

// EXAMPLE IN ACTION:
let darkGray = setRGBa( myColors.darkGray.rgba, '0.75' );
```


---


## Project Workflow

Because the system compiles a full HTML library site along with the extended Bootstrap 4 CSS/JS files the library site uses, there is a lot going on under the hood.

Working with the system generally revolves around two types of uses. You either update settings (using the client-side tool in the rendered site files) or add new items to your system Nunjucks library files and/or Bootstrap integrated SASS files. Either way, you re-render the library site (and generally host it for the team to use from any device).

Some folks like to host the site on a subdomain, and others as a subdirectory. Devs can simply install it locally and work from their workstation.

Here's a diagram to illustrate the intended workflow:

<img src="https://library.mattmct.com/images/obebs4-build-big-picture.jpg" alt="OBE:BS4 Build Process - The Big Picture" width="100%">

It's worth noting, that new projects and prototypes aren't necessarily a part of the library. To try out new ideas, it's best to use a boilerplate provided by the web design system, with a fresh HTML file. However, when creating new components or element variations, you often will want to add your awesome creation into the library for your team and projects to use freely.

*(More on extending the library with your own components/elements as the project matures a bit past this intial alpha stage! See the roadmap section for more!)*

### Project Directories

This project consists of 3 project directories and a handful of process files, that are intended to be a part of your project's root directory. 

- obebs4
    - core
        - css
        - images
        - js
    - data
    - prismjs
        - css
        - js
    - scss
        - mixins
        - settings
        - utilities
- library
    - css
    - images
        - favicons
    - js
- nunjucks
    - data
    - pages
    - templates
        - partials
            - boilerplates
            - colors
            - defaults
            - extensions
            - icons
            - layouts
            - macros
            - reference
            - settings
- package.json, gulpfile.js, etc.

<!--- 
### Project Build Tooling

(Coming Soon!)
-->


---


## Installation

<!--- 
There are two basic ways to install the OBE:BS4 Web Design System. One method is to use Node.js/NPM to install the project as a node module from your console. The other way is to 'old school' download the project zip from here on GitHub, and then copying any necessary extracted files/directories into your project's root folder.
-->

You'll need to use Node.js/NPM to install OBE:BS4 as a node module through your workstation's console.

To really start using your Web Design System however, you'll need to use an OBE:BS4 Settings Tool page to get the JSON settings to customize your Web Design System. (Coversely you could also get your JSON settings from the project's offical example [OBE:BS4 Settings Page](https://library.mattmct.com/settings.html)).

Then you'll need to use Gulp to run the scripts needed to apply your settings and re-generate the HTML, CSS, and JS files for your library. Then you are ready to use your Web Design System to make amazing web stuff!

*NOTE: This project uses Gulp to manage and generate the Web Design System Library Site. So if you are already using Gulp, be sure to not override your gulpfile.js file with the OBE:BS4 gulpfile!*

<!--- 
### Installing via Zip

(Coming Soon!)
-->

### Installing via NPM

**Step 1**: Create a new directory for your project, and navigate to your new project directory in your console.

**Step 2**: Initialize NPM, and fill out your project info for your package.json file as prompted by NPM.
```bash
npm init
```

**Step 3**: Install obebs4 from GitHub (NPM will install all dependencies along with a directory called 'obebs4' inside your 'node_modules' directory)
```bash
npm install --save oberocks/obebs4#master
```

**Step 4**: Open up the OBE:BS4 Settings Page
```bash
open node_modules/obebs4/library/settings.html
```

**Step 5**: Use the OBE:BS4 Settings Page to set your colors and choose the options you want included in your library and brand CSS/JS files. Click the 'GET JSON & LINK' button to get your OBE:BS4 JSON settings. (See [Project Color Wheel](#project-color-wheel) for more info!)

**Step 6**: Create a new file (should be in your project's root directory) called: obebs4_settings.json
```bash
touch obebs4_settings.json
```

**Step 7**: Now paste in your OBE:BS4 JSON settings into your newly created obebs4_settings.json file, and save the file.

**Step 8**: If you don't have a gulp file in your project yet, just run this command to add it from the OBE:BS4 module files:
```bash
cp node_modules/obebs4/example-gulpfile.js gulpfile.js
```

**Step 9**: Now it's time to compile your library site! To do that, run the following gulp command in your console:
```bash
gulp obebs4
```

**Step 10**: Open up your home page:
```bash
open library/index.html
```
Or your boilerplate page ;)
```bash
open library/boilerplates.html
```


---


## Updating Versions

You'll often find yourself in a position to update your OBE:BS4 web design system to get the newest goodies available in your current project. To update the system, use the following command(s):
<!---
### Updating OBE:BS4 Build Dependencies

Before updating your OBE:BS4 system, you'll want to ensure your project has all of the build dependencies for the OBE:BS4 build process scripts. Use the following commands to ensure your project dependencies are up to date:

Bootstrap:
```bash
npm install bootstrap@latest --save
```

jQuery:
```bash
npm install jquery@latest --save
```

Prism.js:
```bash
npm install prismjs@latest --save
```

jQuery DataTables:
```bash
npm install datatables.net@latest --save
```

jQuery BS4 DataTables:
```bash
npm install datatables.net-bs4@latest --save
```

TinyColor 2:
```bash
npm install tinycolor2@latest --save
```
-->

### Updating OBE:BS4 to Latest Version

First use npm install:
```bash
npm install oberocks/obebs4#master --save
```

### Updating OBE:BS4 Build Scripts for Gulp

If your project is using Gulp in any way, you won't want to overwrite your project's build scripts with the OBE:BS4 gulp file scripts! In this case, you'll need to use the first command from the following options:

**If Project IS using Gulp**: you'll just want to open the file and manually copy over the new `gulpfile.js` scripts to your project `gulpfile.js` file using:
```bash
open node_modules/obebs4/example-gulpfile.js
```

**If Project IS NOT using Gulp**: Then simply update your current OBE:BS4 `gulpfile.js` file to the new one with:
```bash
cp node_modules/obebs4/example-gulpfile.js gulpfile.js
```

### Updating OBE:BS4 obebs4_settings.json file

While this project is in an alpha stage, whenever changes are made to the default `obebs4_settings.json` project file, and you are already using an `obebs4_settings.json` file in your project, you might want to update the `obebs4_settings.json` file manually - allowing you to run the library generation script and see these settings reflected correctly in the Library Settings Page.

The following changes were made to the default `obebs4_settings.json` file during the BE:BS4 v0.8.* upgrades:
```json
"enable-caret": "true",
"enable-rounded": "true",
"enable-shadows": "false",
"enable-gradients": "false",
"enable-transitions": "true",
"enable-prefers-reduced-motion-media-query": "true",
"enable-grid-classes": "true",
"enable-pointer-cursor-for-buttons": "true",
"enable-print-styles": "true",
"enable-responsive-font-sizes": "false",
"enable-validation-icons": "true",
"enable-deprecation-messages": "true",
```

```json
"color-50-lighten-percent": "30%",
"color-100-lighten-percent": "20%",
"color-200-lighten-percent": "15%",
"color-300-lighten-percent": "10%",
"color-400-lighten-percent": "5%",
"color-600-darken-percent": "5%",
"color-700-darken-percent": "10%",
"color-800-darken-percent": "15%",
"color-900-darken-percent": "20%",
```


<!---
## Customizing Your Web Design System

(Coming Soon!)

### Bringing System Directories to Root

(Coming Soon!)

### Adjusting the Gulp File

(Coming Soon!)

### Library Site Files

(Coming Soon!)
-->

---



## Roadmap

* Extending The Library Walk-Thru
