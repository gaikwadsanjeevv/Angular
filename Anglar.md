##### JavaScript is a scripting language used to build dynamic and interactive content on websites. It runs in web browsers.  
##### TypeScript is a superset of JavaScript developed by Microsoft that adds static typing, interfaces, and modern object-oriented features.  
##### Angular is a TypeScript-based front-end web application framework developed by Google for building Single Page Applications (SPAs).  
Angular 2 (released in 2016) is the first version that was completely written in TypeScript.  
MongoDB, Node.js, and Angular we would be using together.  
- MongoDB is an open-source NoSQL (also referred to as a non-relational or document-oriented) database that represents and stores data in JSON-format documents. Relational databases such as Microsoft SQL Server, MySQL, and PostgreSQL represent and store data in tables using rows.  
- In relational databases, each table has a schema that defines the columns and data types for each row in the table. In non-relational or document-oriented databases, there’s no defined schema, and every document can be structured differently. This gives non-relational databases more flexibility with documents. This doesn’t mean that non-relational databases are better than relational databases.
- Node.js is an open-source, cross-platform run-time environment for executing JavaScript code server-side. Historically, JavaScript was used for client-side scripting with scripts embedded in a webpage’s HTML.Node.js enables JavaScript to script server-side and potentially produce dynamic web page content before a page is sent to a user’s browser.  
 Before Node.js:
Web development was split between two languages:  
Frontend (browser): JavaScript  
Backend (server): Java, PHP, Python, Ruby, etc.  
This meant developers had to switch between two completely different ecosystems, syntax, and logic.

 After Node.js:  
Node.js allowed JavaScript to run outside the browser, on the server.  
This made it possible to build:  
Frontend using JavaScript (React, Angular, Vue)  
Backend (server-side) using Node.js (Express.js, NestJS, etc.)  
✅ Result:  
You can now build entire full-stack applications using just JavaScript.  

Node.js allows JavaScript to be used for both frontend and backend development, eliminating the need to learn different server-side languages.  
When we set up our API, we’ll be using npm to install some packages that were used to build our Angular application’s API.  

##### Angular provides features for writing modern web applications. These include:  
- A file structure to organize our application  
- A command-line interface that creates files.  
- Modules and components to group our HTML, CSS, and client-side scripting (TypeScript/JavaScript)  
- Forms for gathering user input  
- Services to interact with 3rd party APIs  
- Routing for our application’s various pages.  
<img width="941" height="366" alt="image" src="https://github.com/user-attachments/assets/157c2c9e-9fa5-4e12-8f4b-6eae2ec4872e" />

- Angular is a javascript framework and not an programming language.  
- Like it will provide predefined methods and class for creating API.  
<img width="927" height="387" alt="image" src="https://github.com/user-attachments/assets/55dcb759-4b7d-4843-b1a1-fc1919a51056" />
<img width="885" height="312" alt="image" src="https://github.com/user-attachments/assets/df90b01f-26b3-4237-8ab4-82e83433e5e1" />
<img width="945" height="418" alt="image" src="https://github.com/user-attachments/assets/0580d91d-d7c6-4736-8f60-4a548f446fa3" />

### Creating Angular Project.  
- Node JS  
- Angular CLI  
- Creating project  
- Compile and run
<img width="881" height="307" alt="image" src="https://github.com/user-attachments/assets/074c9479-63db-494f-9c90-8b8f498305ac" />
<img width="987" height="581" alt="image" src="https://github.com/user-attachments/assets/cc0f783d-ec11-4b6e-adff-9cba440f4911" />
<img width="947" height="327" alt="image" src="https://github.com/user-attachments/assets/d0451fde-3ef7-4b51-b294-acd248746244" />
#### - Make a new file : ng new angular-ekart
- Run:        'ng serve'

- We are using Angular to generate dynamic content.
- We have app-root component in index.html rendering the template page so if you see App folder you fine 4 important files.
   - app.ts  
   - app.html  
   - app.css  
   - app.spec.ts   //we write here unit test cases.
  ** Value of selector in app.ts file of component can be used as HTML tag. We have a HTML file content and it is rendered on screen.
     "@Component({  
  selector: 'app-root',  
  imports: [RouterOutlet],  
  templateUrl: './app.html',  
  styleUrl: './app.css'  
 
})"  

- So in app.html we tried to render the data dynamically also called data binding.
   <h2>welcome to {{title}}</h2>  
   Here the title is rendered from the app.ts file in class and we can change the value to render on the screen.  
-  — in an Angular app, the TypeScript code you write in files like app.ts, app.component.ts, services, etc., gets compiled (transpiled) into JavaScript during the build process, and then this JavaScript is what runs in the browser.
-  Does Type Safety Remain After TypeScript is Converted to JavaScript?  
👉 No — type safety is removed during compilation.
1. TypeScript provides type safety at compile-time (development phase):

##### Folder Structure:  
 - a) Node Module - all 3rd party libraries are stored here. We dont deploy on production server. It is purely for development purpose.
 - if we delete the folder then we can bring back by 'npm install' in terminal and the folder is back with all dependencies required for the project+ Extra other Libraries.    
 - b) So how do we know on which packages the angular project is dependent upon - package.json.
 - It contain dependencies and dev dependencies: Dependencies are those on which our project is directly dependent. While the devdependencies is the angular project is dependent on which we are developing the project may need while developing.
 - c) editorconfig - use to set up team environment. There are rules given by team lead he define the coding rules.
 - d) .gitignore - helps to keep those file and folder which can be ignored in git repo.  
 - d) Example in Temp -  i may keep some info or design so i can ignore this file.
 - f) angular.json - very imp file- contails all confuration of the project.
 - g) package-lock.json- records exact versions of every installed dependencies including its subdependencies and there versions. We may be installing the Angular app in production, integration, development environment so so make sure the all dependencies versions remain same.
    - Development is for local coding and testing with full debugging support. Integration is for QA/testing teams to test features in a shared environment using real APIs.Production is the live version for end users, optimized, secure, and without debugging tools.
 - h) tsconfig.json - contains bunch of setting for the typescript compiler this is responsible to convert to javaScript to compile and run.
 - i) SRC - very important folder.
      - IN angular project we can make multiple application, by default we get one that is App. We have 4 component file making an component. Every angular app must have an 'module and copoment'.
   - j) assest folder we store static public resources like images, document.  

  #### Bootstrapping angular application - is process of initializing or loading angular application.  

  - when we do 'ng serve' it generates some bundles and injects into index.html.  But we cannot see those bundles so build the project by 'ng build'. We get to see a new filder created dist and it has 'index.html' where you can see those style files got injected.  
- In angular application webpack traverses through looking for javaScript and other files and it merges them into one bundle javaScript file.  
- In angular - Entry point the angular comes to know from Angular.json file - 'Options'  
- In Index.html is polyfills file in script is used to: Not all browsers are compactible to modern javaScript so to make it comfortable we use polyfill.
-  As we want to run the programme in browser we mention here platform-browser-dynamic.
-  if we wanted to run in mobile then we have use platform-native-dynamic
-  Every application has a module and when the application starts the 


#### What is typescript.  
- Free and open source programming language developed by microsoft, Superset of javaScript.
- When we compile TypeScript - convert to javaScript- and can be run on browsers.
- TypeScript has advantages- Strongly typed.
- Has some OO features.
- Catch errors at compile time.

##### What is a component.  
- Key feature - Angular is said to be component based javaScript framework.
- Every Angular App has atleast 1 component - root component.
  App component is root component and insert all the component in it: Header, navbar, Main(cover, content, subscribe), footer, sideba(popular course 1, popular course 2, popular course 3)

  ###### How to create a component:
  - Create a TypeScript class & export it.
  - Decorate the class with @component decorator.
  - Declare the class in main module file.  

All components are created in the App folder- lets start with header- so lets make a folder 'Header' and a file inside it whose naming convention would be 'filename.component.ts' Inside the file create a typeScrpt class- convention is :  export class HeaderComponent {}  

======================================================================================================  
Why to use Angular.  
- With Aangular you can write declarative code.
  - we write code in form of components.
  - Simplify the process of building complex interactive web user interfaces.
  - Angular uses mostly typeScript which make sure the run time type safety errors wont occur.
  ###### Angular CLI used to allow develop, test, deploy, maintain angular application from CMD.
  - npm install -g @angular/cli  
  - ng version  
  - Node Js Installation.  
  - ng new first-angular-app
  - Some extensions may be helpful to write the code in VSCODE.  
 <img width="1156" height="247" alt="image" src="https://github.com/user-attachments/assets/b54edd7f-53ae-4904-a2ce-99f3219dd3d9" />
 <img width="1220" height="238" alt="image" src="https://github.com/user-attachments/assets/86ac2213-3329-4abf-840d-ed77f8ff2c03" />
 - npm start
<img width="1288" height="497" alt="image" src="https://github.com/user-attachments/assets/79da0f32-510f-4082-b87f-11e4a0b53cb0" />  
<img width="1192" height="627" alt="image" src="https://github.com/user-attachments/assets/be92b8c1-3e73-4b18-aace-586d2a80bc7e" />

### Angular Essentials.  
<img width="1242" height="512" alt="image" src="https://github.com/user-attachments/assets/5b3dd663-e0b7-4aa0-a912-586461d87747" />  
- The files which we see in the root structure in image are essentially configuration file.
<img width="1282" height="558" alt="image" src="https://github.com/user-attachments/assets/fb14a2fa-bd13-4527-bd50-035cf3aed5ee" />
<img width="1228" height="703" alt="image" src="https://github.com/user-attachments/assets/f4ffebbe-21a3-45e2-b5bd-04d057bcba60" />

Think of your Angular app as a tree 🌳:  
Root NgModule = The trunk — the first thing connected to the soil (Angular runtime).  
Feature Modules = Branches that grow from the trunk.  
Components = Leaves that display the UI.  
If you cut the Root NgModule, the whole tree dies — because nothing else has a starting point.  
Why Angular Needs This  
When Angular starts, it needs to know:  
Which components exist in the app.  
Which services are available globally.  
Which first component to put on the screen.  
All of this information is declared in the Root NgModule — in most projects, this is AppModule.  

index.html — only HTML file actually loaded by the browser  
→ Angular finds <app-root> placeholder  
→ Angular replaces <app-root> with the root component’s rendered HTML  

main.ts — entry point that starts Angular  
→ calls platformBrowserDynamic().bootstrapModule(AppModule)  
→ loads the Root NgModule  

AppModule (Root NgModule) — declares/imports app pieces  
→ bootstrap: [AppComponent] tells Angular which component to render first  

AppComponent (Root Component) — has selector: 'app-root'  
→ matches <app-root> in index.html  
→ its template is rendered into the page  

Result  
- index.html loads → main.ts bootstraps AppModule → AppModule bootstraps AppComponent → AppComponent fills <app-root> → app UI appears  








