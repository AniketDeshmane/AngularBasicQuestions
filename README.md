## NPM, NVM and Angular CLI
```
https://github.com/coreybutler/nvm-windows (get nvm from here)
```
```
C:\Users\<Username>\AppData\Roaming\nvm  	--Can access nvm here in windows
```

```
nvm list						--list all the node versions
```

```
nvm install <node_version>      		// Install a specific Node version
nvm install node                		// Install latest Node release (Current)
nvm install --lts               		// Install latest LTS release of NodeJS
nvm install-latest-npm          		// Install latest NPM release only
```
```
nvm use 20.17.0	   --use specific node version 
npm install -g @angular/cli  --install angular cli
npm install -g @angular/cli@12.2.18  --specific angular version
ng version   --check cli version
```

To create any project 
```
ng new <project-name>
```


To start the project from github

```
npm install && npm start
ng serve
```

## Question and Answer

What is a selector and Template?

A selector is used to identify each component uniquely into the component tree.
```
@Component({
  selector: 'app-root',
  standalone: true,
  imports: [RouterOutlet],
  templateUrl: './app.component.html',
  styleUrl: './app.component.css'
})
```
In html file we can access the selector like below

```
<app-root></app-root>
```
Template is nothing but the html view, its the UI on which the user interact.

```
templateUrl: './app.component.html',
```
We can point the templateUrl to a html file or directly add the html in the templateUrl tag
```
import {Component} from 'angular2/core';
@Component({
    selector: 'my-app',
    template: `
    <h1>My First Angular 2 multiline template</h1>
    <p>Second line</p> 
    `
})
export class AppComponent { }
```
