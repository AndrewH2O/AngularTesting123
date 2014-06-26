# Setting up Angular in VS2012 using Chutzpah

After much fiddling got this to work... in retrospec looks simple now.


## Project is based on angular phone catalog tutorial

see origREADME.md for details directories just added as a web project. I have ripped out some pieces however.

## Project Pre-Requisite

Install bower packages (bower install) - bower.json unpacks into bower_components

## Chutzpah piece

Requires the Chutzpah extension installed in visual studio
Set up Chutzpah.json see - route folder

Contents show paths etc - used instead of SpecRunner.html

    
```    {  

       "Framework": "jasmine",

       "RootReferencePathMode":"SettingsFileDirectory",
       "References": [
		{ "Path": "/app/bower_components/angular/angular.js"},
		{ "Path": "/app/bower_components/angular-mocks/angular-mocks.js"},
		{ "Path": "/app/js/controllers.js" }
	],

	"TestHarnessDirectory": "/test/unit/",
    	"Tests": [ "/test/unit/* ], 

    }
    ```
## Test Explorer

Open test explorer and run jasmine PhoneCat controllers test


