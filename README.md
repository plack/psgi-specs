This is PSGI, Perl Web Server Gateway Interface -- ala Python's WSGI and Ruby's Rack.

[PSGI protocol specification](http://github.com/miyagawa/psgi-specs/blob/master/PSGI.pod) is currently in draft. We're reviewing feedbacks before making it final. See also [FAQ](http://github.com/miyagawa/psgi-specs/blob/master/FAQ.pod)

## Web Servers

* [Plack](http://github.com/miyagawa/Plack) contains server side implementations such as CGI, FastCGI, mod_perl and perl-based web servers like HTTP::Server::Simple, AnyEvent, FastCGI::EV and Mojo.
* [nginx](http://www.nginx.eu) with [Yappo's patches](http://github.com/Yappo/nginx-psgi-patches) can run a PSGI application on Perl embedded in the nginx web server.

Following web servers are planned to be supported, or authors are in contact to support PSGI:

* [mod_perlite](http://github.com/sodabrew/mod_perlite/)
* [Perl Google App Engine](http://code.google.com/p/perl-appengine/)

## Supported Web Application Frameworks

* [Catalyst](http://www.catalystframework.org/) runs as a PSGI application using [Catalyst::Engine::PSGI](http://github.com/miyagawa/Catalyst-Engine-PSGI).
* [Angelos](http://github.com/dann/angelos) has a Plack support by default
* [Ark](http://github.com/typester/aerk-perl) has a PSGI/Plack support branch
* [HTTP::Engine](http://github.com/http-engine/HTTP-Engine) now has a thin wrapper interface to write a new micro web server on PSGI
* [Dancer](http://github.com/sukria/Dancer) now runs as a PSGI application by default
* [Schenker](http://github/com/spiritloose/Schenker) runs fine as PSGI app since it uses HTTP::Engine
* [CGI::Application](http://cgi-app.org/) runs as a PSGI application using [CGI::Application::PSGI](http://github.com/miyagawa/CGI-Application-PSGI)
* [CGI.pm](http://search.cpan.org/dist/CGI) has a native PSGI support to get parameters in [miyagawa's fork](http://github.com/miyagawa/CGI.pm)
* [Squatting](http://github.com/beppu/squatting) runs as a PSGI application using [Squatting::On::PSGI](http://github.com/miyagawa/Squatting-On-PSGI)
* Arbitrary plain CGI scripts can be run as a PSGI application using CGI::Emulate::PSGI emulation layer.

Planned frameworks:

* [Jifty](http://jifty.org/)
* [Sledge](http://sl.edge.jp/)






