# Documentation

Documentation is the most important step and is required for every build. It doesn't take more than 15 minutes and it's great to lay out your toolkit so there are no surprises later on in the build. Get this out of the way, first. Make changes as you go along.

TLDR; Categories Required:

- Browser Support
- Technologies Used
- Compatibility Notes
- Environment Setup Instructions 
- Dependencies Used
- Additional Notes/Information

## Browser Support

Provide **all** documentation within the project.

**Most projects will be IE9+**

- Check to make sure - don't shoot yourself in the foot by going with an IE9+ utility only to realize you need IE8 support

**List out complete browser support inside the README.md**

- If you're not sure about something, ask your account manager to **send you an email**.
- There is a difference between Chrome on an IPhone and Android. There are differences between Android Phones, etc.


### Currently Supported Browsers:
- IE 9+ 
- Chrome 20+
- Firefox 7+
- iOS 6+ Mobile Safari
- Android 4.x+ Browser
- Android Chrome Browser (Edge)
- Safari 6+ (OSX)

## Technologies 

List out the utilities / frameworks you're going to be using for the project. If there are any issues, or technologies in question, list these under compatibility notes.

- SCSS 3.3+ (Ruby)
- Angular JS 1.3+ (IE9+)
- jQuery 1.10.0 (_see compatibility notes_)
- Font Awesome (4.2.1) (IE9+)

## Compatibility Notes 

If there is something that doesn't fall under an assumption, list it here

## Environment Setup

### Development Dependencies

If you find yourself using a specific toolset for your development environment, make sure to list it here. If you're using a package.json file and/or bower.json, run ```npm shrinkwrap``` to lock in the version of whatever project you're using.

List your dev dependecies that you've got inside your package.json / bower.json. Run ```npm shrinkwrap``` before you're done to lock in the correct version. There will be times where a project will break if dependencies do not have a correct version number. Bower does not currently have this implemented but will soon [Bower Issue #1362](https://github.com/bower/bower/issues/1362)

### Common Development Dependencies
- Node
- Grunt (task runner)
- Gulp ( new task runner)
- SCSS ( css pre-compiler)
- Bower (package dependency manager)
- Jasmin
- Karma

## Getting Up and Running

Any commands that require execution

- ```npm install```
- ```bower install```


# Project Setup & Scaffold

- Create a GIT repo on Bitbucket.
- Project Directory Tree should mimic what the industry does for JS projects
- Use a *real* IDE. Although we shouldn’t discriminate by text editor, IDEs that save time and money are what business owners are looking for. The greater industry of development also appreciates everyone knowing the top tier IDEs.

#### Common Editors / IDE's You'll see 
- Netbeans
- Sublime Text
- Webstorm
- VIM

## Scaffolding Out a Project (TBD)

### Angular Projects:

- [Yeoman - AngularJS](https://github.com/yeoman/generator-angular)
	- [Google AngularJS Best Practies Recommendations](https://docs.google.com/document/d/1XXMvReO8-Awi1EZXAXS4PzDzdNvV6pGcuaF4Q9821Es/pub)

### Lightweight Projects:
- [Yeoman - Gulp-webapp](https://github.com/yeoman/generator-gulp-webapp)
	- [Recipes will make your life easier](https://github.com/yeoman/generator-gulp-webapp/blob/master/docs/recipes/README.md)
	
Includes:

- Gulp
- Sass
- Bootstrap (chances are you won't need this)
- Modernizr

Any additional components are installed as easily as running bower search and install:

-  ```bower search jQuery``` 
-  ```bower install jQuery --save```

Learn more about installing and using Yeoman [here](http://yeoman.io/learning/index.html).


## Directory Structure
<pre>
	app/
		images/
		scripts/
			main.js
			config.js
			controllers/
			constants/
			directives/
			enums/
			filters/
			services/
		scss/
			core/
			deps/
			components/
			theme/
		views/
			index.html
	package.json
	bower_components
</pre>



## GIT Early, GIT Often

We cannot stress this enough. GIT After Every:

- Module
- Component
- Feature
- 10 LOC (as an extreme example)

## DO NOT commit after a full day's of work.

## Consistent Nomenclature
- CSS / HTML
  - https://google-styleguide.googlecode.com/svn/trunk/htmlcssguide.xml
  - BEM, SMACSS, or similar naming conventions

```

	.bio {
		
	}
	
	.bio-image {
		width:200px;
		height:200px;
	}
	
	.bio-image-small {
		width:100px;
		height:100px;
		
	}
	
```



- Javascript
  - [Google JS Styleguide](https://google-styleguide.googlecode.com/svn/trunk/javascriptguide.xml)
  - [Airbnb JS Styleguide](https://github.com/airbnb/javascript)

## Recommendations
- Use popular technologies. Going rogue will only cause problems for new devs on a project and could cause potential problems when doing research
  - SCSS
  - Yeoman
  - Coffeescript
  - Angular JS
  
## Maintainability
- Follow existing standards
  - If there’s an opportunity to improve that is a low effort/cost: Improve it
  - Develope under the assumption you are not the one maintaining the code base

## Modulization of CSS/JS/HTML
See /examples folder 

### Component Principles to Follow

- Self contained
- One Thing Very Well
- Extensible
- Defined at any degree
  - e.g.: Responsive Wrapper, Header, navigation, primary button
- Reuse other components as much as possible
- Use Bower to Handle Components when possible



# Time Estimation
## Reconnaissance
- Gathering Information about a Project
- The more details about the Project the better, assumptions create risk

## Company evaluation
- Business Evaluation
	- Business
		- how many hours have been predefined? Does that align with what you think that might take?
		- What’s the purpose / what are you trying to solve?
	- Technical
		- How long will it take to create using a certain library/utility/framework?
	- Creative
		- Design direction and UX recommendations
	- Complexity Level from all 
	- Risks and Opportunities
- FED Evaluation
	- Browser Compatibility
		- **Ask for browser support. OSX vs Windows. There’s a difference between Firefox on Mobile and in the browser. Get a defined list.**
		- Responsive Principles
		- Frameworks to leverage
			- Grid frameworks like Susy vs whipping up your own
	- Research & Development

## Scoping Requirements and hourly Estimation

- Estimation Overview
	- Calculate hours on all requirements
	- Calculate hours and add padding on certain risks
	- Add padding for certain levels of complexity
		- browser support
		- creating new ideas
- Breakdown scoped requirements for estimation
	- Componetize Everything
	- Headers
	- Footers
	- Side Bar
	- Navigation
- Secondary Requirements
	- Padding for potential browser compatibility issues
	- Padding for potential responsive defects
	- PITA Padding
- Solutions for Potential Risks
	- Coming up with Fallbacks:
		- Plan A (CSS3)
		- Plan B (JQuery)
		- Plan C (Escalating to Higher Power)
			
# Work Ethic

## Consultation for Self and Others
- Proactive
	- Reach out and help provide a solution to potential problem areas
- Provide **at least two** solutions to any given problem
	- See "Solutions for Potential Risks"
- Ability to consult to any discipline
## Understanding Multiple Disciplines
- Creative
	- Tools
		- Photoshop Workflow
		- Sketching
		- Wireframing
	- Creative Process
		- User Personas
		- Usability
	- Business Objectives
		- Scoping
		- Budget
- Backend
- Dev Ops
- Production
- Support
		
# Continuous Self Learning
## Staying Up-to-date
- [http://html5rocks.com](http://html5rocks.com)
- [http://thechangelog.com/](http://thechangelog.com)
- [http://docs.webplatform.org/wiki/Main_Page](http://docs.webplatform.org/wiki/Main_Page)
- [http://tympanus.net/codrops/](http://tympanus.net/codrops/)
- [http://superherojs.com/](http://superherojs.com/)
- [http://www.sitepoint.com/](http://www.sitepoint.com/)

## Community Leaders
- [http://paulirish.com](Paul Irish)
- [http://addyosmani.com](Addy Osmani)
- [http://www.nczonline.net](Nicholas Zackas)

## Latest Utilities/Frameworks And When To Use Them
- AngularJs, jQuery, etc
	- [http://docs.angularjs.com](Angular JS Docs)
	- [http://egghead.io](Egghead.io)
	- [http://docs.jquery.com](Jquery Docs)
- Knowing Resources Available for Research
	- Stackoverflow
	- IRC/Twitter
		- Plenty of great channels for instant help
		
## Understanding Latest Techniques
- Compatible CSS from IE8 to Chrome
- Responsive (breakpoints) vs. Adaptive (device)
- CSS Animations & Effects
- Performant Alternative Solutions (Choosing the right library)
	- Is Jquery really worth it?
	- Onloading GPU

## Responsive Implementations
- Desktop First
	- Prototype mobile HTML layout but leave functionality and styling to the end
- Mobile First
	- [MDN - Mobile First](https://developer.mozilla.org/en-US/Apps/app_layout/Mobile_first)
	- [Google - Responsive Design Patterns](https://developers.google.com/web/fundamentals/layouts/rwd-patterns/)
	
## Performance
- Stress / Smoking Testing
- Proficiency in ALL Dev tools for each browser
- Proficiency in using profiling tools and understanding data

## FED Philosophy
- FED is an expert in the fields a full stack developer is only familiar with
- Identifying potential issues with a design that might have poor usability
- Find a time to share knowledge (1hr meetings to discuss projects, new technologies, etc.)

## Code Reviews
- Developers should review their own code and peer review others. MAX 15 minutes for yourself and MAX 15 minutes for others. 
- This should be done on a daily basis (Don't GIT a whole day's worth of work!)
