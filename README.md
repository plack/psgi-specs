This is PSGI, Perl Web Server Gateway Interface -- ala Python's WSGI and Ruby's Rack.

[PSGI protocol specification](http://github.com/miyagawa/psgi-specs/blob/master/PSGI.pod) is currently in draft. We're reviewing feedbacks before making it final. See also [FAQ](http://github.com/miyagawa/psgi-specs/blob/master/FAQ.pod)

## Web Servers

* [Plack](http://github.com/miyagawa/Plack) contains server side implementations such as CGI, FastCGI, mod_perl and perl-based web servers like HTTP::Server::Simple, AnyEvent, FastCGI::EV and Mojo.
* [nginx](http://www.nginx.eu) with [Yappo's patches](http://github.com/Yappo/nginx-psgi-patches) can run a PSGI application on Perl embedded in the nginx web server.

Following web servers are planned to be supported, or authors are in contact to support PSGI:

* [mod_perlite](http://github.com/sodabrew/mod_perlite/)
* [Perl Google App Engine](http://code.google.com/p/perl-appengine/)

## Supported Web Application Frameworks

* [Catalyst](http://www.catalystframework.org/) with [Catalyst::Engine::PSGI](http://github.com/miyagawa/Catalyst-Engine-PSGI).
* [Squatting](http://github.com/beppu/squatting) with [Squatting::On::PSGI](http://github.com/miyagawa/Squatting-On-PSGI)
* [HTTP::Engine](http://github.com/http-engine/HTTP-Engine) with HTTP::Engine::Interface::PSGI
* [Dancer](http://github.com/sukria/Dancer)
* [CGI::Application](http://cgi-app.org/) with [CGI::Application::PSGI](http://github.com/miyagawa/CGI-Application-PSGI)
* [CGI::PSGI](http://github.com/miyagawa/CGI-PSGI) is a CGI.pm subclass that runs under PSGI environments
* [Continuity](http://github.com/awwaiid/continuity)
* [Angelos](http://github.com/dann/angelos)
* [Ark](http://github.com/typester/aerk-perl)
* [Schenker](http://github.com/spiritloose/Schenker)
* [Noe](http://github.com/yusukebe/Noe)
* [Kamui](http://github.com/nekokak/p5-Kamui)
* Arbitrary plain CGI scripts can be run as a PSGI application using CGI::Emulate::PSGI emulation layer.

Planned frameworks:

* [CGI.pm](http://search.cpan.org/dist/CGI) - though we already have CGI::PSGI and CGI::Emulate::PSGI
* [Jifty](http://jifty.org/)
* [Sledge](http://sl.edge.jp/)






