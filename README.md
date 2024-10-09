Scaffolding 
----------

node_modules :  This directory contains all the dependencies and packages installed via npm

package.json :  the project dependency distrubution file

public  - Where we can keep the static assets served via too level

pages   - Most important part of next js app
        - Each file represents a route in the application since next js uses file based routing 
        - index.js represents the root route  ( '/')  Entry point of Application
        - _app.js Custom App component used to initialize the pages 
          enables the navigation between the pages. if you want to inject any global styles and layouts we can do this here
        _document.js  This custom document component is used to      augmemnt the application HTML and body tags, seeting up the meta tags , fonts linking , global scripts
        api/ - special sub directory used to create API routes 
        you can create endpoint by placing a JS file 

        Why _  in next.js project

        The underscore _prefix int the files like _app.js _document.js
        _error.js etc in next.js serves as a convention to indicate that these files have a special purposes within framework

        The underscore (_) indicates that these files are tied to the internal workings of the Next.js framework.you can custimize them

        _ files are not routable but influence the behaviour of the route

        its avoids route conflicts


styles/ 

        The directory is used for blobal styles and css modules 

        global.css  - contians the global css rules usually imported in import "@/styles/globals.css";

        Home.module.css - css scoping based on components in this case Home component


.gitignore - This file specifies which files and directories should be ignored by Git. The default .gitignore file includes node_modules/, .next/


package.json used for scripts and dependencies

next.config.js -- File is used to customize the configuration of next js app

jsconfig.json --jsconfig.json file is used to configure JavaScript settings for your project. absolute imports, path aliases, and IntelliSense for your code editor (majorly for developer experience ) cleaner imports 
