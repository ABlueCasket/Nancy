# Meet Nancy

Nancy is a lightweight HTTP framework for the .Net platform and Mono. The ethos of Nancy is to strive for simplicity and elegance, all features to be easy and ready to use right out-of-the-box. 

Simplicity means that a feature should requires little or low-ceremony to use, there should always be sensible default configurations, behaviors and conventions available.

The elegance comes from an easy to use and light syntax, combined with letting the framework be responsible for a lot of things that developers should not have to worry about or re-implement in each application you create.

We call this the super-duper-happy-path.

## Features

* Built from the bottom up, not simply a DSL on top of an existing framework. Removing limitations and feature hacks of an underlying framework, as well as the need to reference more assemblies than you need. _keep it light_
* Run anywhere. Nancy is not built on any specific hosting technology can can be run anywhere. Out of the box, Nancy supports running on ASP.NET/IIS, WCF, Self-hosting and any [OWIN](http://owin.org)
* Ultra lightweight action declarations for GET, HEAD, PUT, POST, DELETE and OPTIONS requests
* View engine integration (Razor, Spark, NDjango, dotLiquid and our own SuperSimpleViewEngine)
* Powerful request path matching that includes advanced parameter capabilities. The path matching strategy can be replaced with custom implementations to fit your exact needs
* Easy response syntax, enabling you to return things like int, string, HttpStatusCode and Action<Stream> elements without having to explicitly cast or wrap your response - you just return it and Nancy _will_ do the work for you
* A powerful, light-weight, testing framework to help you verify the behavior of your application

## Usage

    public class Module : NancyModule
    {
        public Module()
        {
            Get["/greet/{name}"] = x => {
                return string.Concat("Hello ", x.name);
            };
        }
    }

## Community

You can find lot of Nancy users on the [Nancy User Group](https://groups.google.com/forum/?fromgroups#forum/nancy-web-framework). That is where most of the discussions regarding the development and usage of Nancy is taking place. You can also
find Nancy on Twitter using the #NancyFx hashtag.	
	
## Help out

There are many ways you can contribute to Nancy. Like most open-source software projects, contributing code
is just one of many outlets where you can help improve. Some of the things that you could help out with in
Nancy are:

* Documentation (both code and features)
* Bug reports
* Bug fixes
* Feature requests
* Feature implementations
* Test coverage
* Code quality
* Sample applications

## Contributors

Nancy is not a one man project and many of the features that are availble would not have been possible without the awesome contributions from the community!

* [Andy Pike](http://github.com/andypike)
* [Bjarte Djuvik Næss](http://github.com/bjartn)
* [Carlo Kok](http://github.com/carlokok)
* [Chris Nicola](http://github.com/lucisferre)
* [David Hong](http://github.com/davidhong)
* [Graeme Foster](http://github.com/GraemeF)
* [Guido Tapia](http://github.com/gatapia)
* [Greg Banister](https://github.com/gbanister)
* [Ian Davis](http://github.com/innovatian)
* [Jonas Cannehag](http://github.com/knecke)
* [José F. Romaniello](http://github.com/jfromaniello)
* [Karl Seguin](http://github.com/karlseguin)
* [Leo Duran](http://github.com/leoduran)
* [Luke Smith](http://github.com/lukesmith)
* [James Eggers](http://github.com/jameseggers1)
* [Jason Mead](http://github.com/meadiagenic)
* [Jeremy Skinner](http://github.com/jeremyskinner)
* [João Bragança](http://github.com/thefringeninja)
* [Johan Danforth](http://github.com/johandanforth)
* [Johan Nilsson](http://github.com/Dashue)
* [Jonathan Scoles](https://github.com/jscoles)
* [John Downey](http://github.com/jtdowney)
* [Jonas Schmid](http://github.com/jschmid)
* [Mark Rendle](http://github.com/markrendle)
* [Maciej Kowalewski](http://github.com/maciejk)
* [Mindaugas Mozûras](http://github.com/mmozuras)
* [Patrik Hägne](http://github.com/patrik-hagne)
* [Pedro Felix](http://github.com/pmhsfelix)
* [Piotr Wlodek](http://github.com/pwlodek)
* [Phil Haack](http://github.com/haacked)
* [Robert Greyling](http://github.com/robertthegrey)
* [Roy Jacobs](http://github.com/RoyJacobs)
* [Simon Skov Boisen](http://github.com/ssboisen)
* [Steven Robbins](http://github.com/grumpydev)
* [Thomas Pedersen](http://github.com/thedersen)
* [Troels Thomsen](http://github.com/troethom)
* [Vidar L. Sømme](http://github.com/vidarls)
* [Nathan Palmer](https://github.com/nathanpalmer)

## Copyright

Copyright © 2010 Andreas Håkansson, Steven Robbins and contributors

## License

Nancy is licensed under [MIT](http://www.opensource.org/licenses/mit-license.php "Read more about the MIT license form"). Refer to license.txt for more information.
