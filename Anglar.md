# Angular  
#### Learn &amp; Practice  
What is Angular  
Javascript framework for web development  
Single Page Application(No Refresh on clicks)  
Developed by Google  

<img width="581" alt="image" src="https://github.com/user-attachments/assets/7740be27-c2cd-459f-ab32-8fb70ff87695" />  


##### NPM (Node Package Manager)
is a tool for managing and installing libraries or packages that you use in your Angular or React project.  
Every Angular or React project needs a set of tools, libraries, and frameworks to work (e.g., Angular framework, React library, testing tools, etc.).
NPM fetches these libraries from its online registry and installs them into your project.  
##### Managing Dependencies  
Each project has a package.json file, which is like a "shopping list" of all the libraries your project uses.  
NPM keeps track of the versions of these libraries and ensures everything is compatible.  
##### Running Scripts  
NPM is also used to run custom or pre-defined tasks, like:  
Starting the development server.  
Building the app for production.  
Running tests.  
##### Updating Dependencies  
NPM makes it easy to update libraries to the latest versions or manage compatibility issues.  
##### Sharing and Publishing  
For developers who create reusable components or tools, NPM allows you to publish your own libraries so others can use them in their projects.  
<img width="576" alt="image" src="https://github.com/user-attachments/assets/788d98b2-8b2a-4468-b7ab-a837f995ac1c" />  
----------------------  
## Installation  
<img width="695" alt="image" src="https://github.com/user-attachments/assets/c8f04e4e-4ec1-47bf-b95e-7a5e9fc0d8f1" />  
--> Download Node.js  
What is Node.js?  
Node.js is a runtime environment that allows you to run JavaScript code outside the browser.  
It’s not a programming language or a server by itself. It is based on the V8 JavaScript engine (the one used in Google Chrome) to execute JavaScript on your computer or server.  
In Simple Terms: Think of Node.js as an engine that powers JavaScript to run wherever you want, not just inside a web browser.  
Angular projects use NPM (Node Package Manager), which comes with Node.js.  
#### Running Angular CLI Commands:  
Angular CLI (ng) is a Node.js-based tool that lets you:  
Create a new Angular project (ng new).  
Serve your project locally during development (ng serve).  
Build your project for production (ng build).  
These commands require Node.js to run.  
got to:  https://angular.io/cli  
> npm install -g @angular/cli
<img width="559" alt="image" src="https://github.com/user-attachments/assets/33fc9576-b294-4b07-9854-e2454746e29f" />

The ng command is part of the Angular CLI and is used to manage, build, and maintain Angular applications efficiently. It simplifies common tasks in Angular development, such as creating a new project, generating components, and serving the application.  
ng is short for Angular, derived from the ng in AngularJS directives like ng-app, ng-model, etc.
It serves as the command-line interface for Angular projects     
> ng new blog  
> cd blog  
> code . //to open in vscode  
> ng serve //will build the project and start running on browser.
<img width="661" alt="image" src="https://github.com/user-attachments/assets/e3bae34f-48ad-44f0-81ca-937a43c2ce07" />
> gives the local address to run project.
> When u install a particular version of angular CLI which installs the latest version, you get to see same angular version in package.json file.
> Now if u want to install an older version of angular then you go ahead and first uninstall the npm cli version, and then install the required version as:
> npm install -gangular/cli@10.0.0  



