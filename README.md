# Photo gallery

<h3>Frameworks - Tools - Libraries</h3>
<ul>
<li>ASP.NET Core</li>
<li>Entity Framework Core</li>
<li>Automapper</li>
<li>Angular 2</li>
<li>Typescript</li>
<li>Bootstrap 3</li>
<li>Gulp</li>
<li>Bower</li>
</ul>

<h3>Installation instructions - Part 1</h3>
<ol>
<li>Install ASP.NET Core according to your development environment from <a href="https://www.microsoft.com/net/core" target="_blank">here</a>.</li>
<li>Install <strong>NPM</strong> by installing <a href="https://nodejs.org/en/" target="_blank">Node.js</a>.</li>
<li>Install Bower, Gulp, Typescript and Typescript Definition Manager globally by typing the following commands on the console/terminal:
<ul>
<li>npm install -g bower</li>
<li>npm install -g gulp</li>
<li>npm install -g typescript</li>
<li>npm install -g typings</li>
<li>npm install -g tsd</li>
</ul>
</li>

<h3>Installation instructions - Part 2</h3>
<ol>
<li>Download and install Visual Studio 2015 from <a href="https://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx" target="_blank">here</a>.</li>
<li>Open Visual Studio 2015 and install any update related to ASP.NET Core (check the notifications).</li>
<li>Download the source code and open the solution.</li>
<li>By the time you open the solution, VS 2015 will try to restore Nuget, NPM and Bower packages.</li>
<li>In case it fails to restore NPM and Bower packages, open a console and navigate at the src/PhotoGallery path where the <i>package.json</i> and <i>bower.json</i> files exist. Run the following commands:
<ul>
<li>npm install</li>
<li>typings install</li>
<li>bower install</li>
<li>gulp build-spa</li>
</ul>
</li>
<li>Open <strong>appsettings.json</strong> file and alter the database connection string to reflect your SQL Server environment.</li>
<li>Open a console and navigate to src/PhotoGallery where the project.json exists. Run the following commands to enable migrations and create the database:
<ol>
<li>dotnet ef migrations add initial</li>
<li>dotnet ef database update</li>
</ol>
</li>
</ol>
