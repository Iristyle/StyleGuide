## Code Style

--

* Use soft-tabs with a 2 space indent
* Maximum 80 characters per line
* Write inline XML documentation for any *public* methods
* [Allman style braces](http://en.wikipedia.org/wiki/Indent_style#Allman_style)
* Build process will enforce using [StyleCop](http://stylecop.codeplex.com/)

## Practices

--

* All code should have accompanying tests as documentation
* Major frameworks / assemblies should have markdown readme in root of repo

## Project Naming Guidelines

--

* Test projects should always end in .Tests as convention to be picked up by
build process

## Frameworks

--

### Testing Frameworks
* [xUnit.Net](http://xunit.codeplex.com/) - Unit testing framework
* [AutoFixture](http://autofixture.codeplex.com/) - xUnit.Net plugin
* [FakeItEasy](https://github.com/patrik-hagne/FakeItEasy) - mocking framework
* [NSpec](http://nspec.org/) - BDD framework for xSpec (context/specification)
style, generally used to model domain behavior
* [NSpec xUnit Adapter](https://github.com/psilvaferreira/NSpecAdapterForXunit)
* [SpecFlow](http://www.specflow.org/) - BDD framework for xBehave (GWT) style
BDD tests, generally used for high level acceptance / feature definitions

Keep in mind that for web applications it may be more beneficial to run tests
via node.js / javascript, but there are a couple of .NET options

* [Plasma](https://github.com/jennifersmith/plasma) - standalone, doesn't
require IIS
* [Lightweight Test Automation Framework](http://ltaf.codeplex.com/) - can
automate running real tests in IE, FireFox, Safari and Opera (like JsTestDriver)

### Test Runners - Pick One
* [Mighty Moose](http://continuoustests.com/) - Automated Continuous Runner
* [NCrunch](http://www.ncrunch.net/) - Automated Parallel Continuous Runner
* [Chutzpah](http://chutzpah.codeplex.com/) - Javascript test runner capable of
running QUnit and Jasmine frameworks with PhantomJS (Mocha and Chai are however
the web frameworks of choice)

VS11 has added runner support via plugins, but does not support continous.

Resharper and CodeRush have runners as well, but at this time, they are not
continous.

### Web Frameworks
* [ASP.NET MVC 4](http://www.asp.net/mvc/mvc4)
* [NancyFx](https://github.com/NancyFx/Nancy)

### REST Services
* [ServiceStack](http://www.servicestack.net/) - Server side
* [RestSharp](http://restsharp.org/) - Client

### Data Access
[Dapper](http://code.google.com/p/dapper-dot-net/)
[ServiceStack.Redis](https://github.com/ServiceStack/ServiceStack.Redis)

### IoC
* [AutoFac](http://code.google.com/p/autofac/)
* [Funq](http://funq.codeplex.com/) - For simpler requirements

### Validation
* [FluentValidation](http://fluentvalidation.codeplex.com/)

### Logging
* [NLog](http://nlog-project.org/)
* [Common.Logging](https://nuget.org/packages/Common.Logging) - Use only
when build frameworks that shouldn't take a specific logging dependency
* [Elmah](http://code.google.com/p/elmah/) - For web projects

### 3rd Party Service Integrations
* [AWS SDK](http://aws.amazon.com/sdkfornet/)

### Additional References
* [Mono](http://www.mono-project.com/Coding_Guidelines)
* [IDesign C#](http://www.idesign.net/idesign/download/IDesign%20CSharp%20Coding%20Standard.zip)
* [Encodo C# Handbook](http://code.msdn.microsoft.com/encodocsharphandbook/Release/ProjectReleases.aspx?ReleaseId=3352)
* [Microsoft Framework Design Guidelines](http://msdn.microsoft.com/en-us/library/ms229042.aspx)
* [Denni's C# Standards](http://csharpguidelines.codeplex.com/)
* [Microsoft's All-In-One](http://1code.codeplex.com/wikipage?title=All-In-One%20Code%20Framework%20Coding%20Standards&referringTitle=Documentation)
* [SharpDevelop](http://www.sharpdevelop.net/TechNotes/SharpDevelopCodingStyle03.pdf)

### StyleCop rules file
* [StyleCop.Settings](https://github.com/EastPoint/StyleGuide/blob/master/csharp/Settings.StyleCop)