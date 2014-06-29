# One North FED Philosophy


## Best Practices

### Documentation
- Provide **all** documentation within the project. High level or all detail documentation should be stored in the README.md
- Everything that needs to happen to set up a working development environment
- If there’s a build step, the command needed to build out the project
- Project Directory Tree should mimic what the industry does for JS projects
- GIT all your files
- Use a *real* IDE. Although we shouldn’t discriminate by text editor, IDEs that save time and money are what business owners are looking for. The greater industry of development also appreciates everyone knowing the top tier IDEs.
	- Netbeans vs Sublime
	
- [Yeoman::Angular::Grunt](https://github.com/yeoman/generator-angular)
- [Yeoman::Angular::Gulp](https://github.com/henyojess/generator-gulp-ng) **

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

## Consistent Nomenclature
- CSS / HTML
  - https://google-styleguide.googlecode.com/svn/trunk/htmlcssguide.xml
  - BEM, SMACSS, or similar naming conventions
    - global-header, bio , bio-image, bio-image-small
- Javascript
  - https://google-styleguide.googlecode.com/svn/trunk/javascriptguide.xml
  - https://github.com/airbnb/javascript

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

- Components should be self contained
- Components should do one thing very well
- Should reuse other components as much as possible
- Components should be extensible
- Components can be defined at any degree
  - e.g.: Responsive Wrapper, Header, navigation, primary button
- **Use Bower to Handle Components when possible** see .bowerrc, bower.json

## Time Estimation
- Reconnaissance
	- Gathering Information about a Project
	- The more details about the Project the better, assumptions create risk
- Company evaluation
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
- Scoping Requirements and hourly Estimation
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
			
## Work Ethic

- Consultation for Self and Others
	- Proactive
		- Reach out and help provide a solution to potential problem areas
	- Provide **at least two** solutions to any given problem
		- See "Solutions for Potential Risks"
	- Ability to consult to any discipline
- Understanding Multiple Disciplines
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
		
## Continuous Self Learning
- Staying Up-to-date
	- [http://html5rocks.com](http://html5rocks.com)
	- [http://thechangelog.com/](http://thechangelog.com)
	- [http://docs.webplatform.org/wiki/Main_Page](http://docs.webplatform.org/wiki/Main_Page)
	- [http://tympanus.net/codrops/](http://tympanus.net/codrops/)
	- [http://superherojs.com/](http://superherojs.com/)
	- [http://www.sitepoint.com/](http://www.sitepoint.com/)
- Community Leaders
	- [http://paulirish.com](Paul Irish)
	- [http://addyosmani.com](Addy Osmani)
	- [http://www.nczonline.net](Nicholas Zackas)
- Latest Utilities/Frameworks And When To Use Them
	- AngularJs, jQuery, etc
		- [http://docs.angularjs.com](Angular JS Docs)
		- [http://egghead.io](Egghead.io)
		- [http://docs.jquery.com](Jquery Docs)
	- Knowing Resources Available for Research
		- Stackoverflow
		- IRC/Twitter
			- Plenty of great channels for instant help
- Understanding Latest Techniques
	- Compatible CSS from IE8 to Chrome
	- Responsive (breakpoints) vs. Adaptive (device)
	- CSS Animations & Effects
	- Performant Alternative Solutions (Choosing the right library)
		- Is Jquery really worth it?
		- Onloading GPU
