This is PSGI, Perl Web Server Gateway Interface -- ala Python's WSGI and Ruby's Rack.

[PSGI protocol specification](http://github.com/miyagawa/psgi-specs/blob/master/PSGI.pod) is currently in draft. We're reviewing feedbacks before making it final. See also [FAQ](http://github.com/miyagawa/psgi-specs/blob/master/PSGI/FAQ.pod)

## Web Servers

* [Plack](http://github.com/miyagawa/Plack) contains server side implementations such as CGI, FastCGI, mod_perl and perl-based web servers like HTTP::Server::Simple, AnyEvent, FastCGI::EV and Mojo.
* [nginx](http://github.com/Yappo/p5-Plack-Impl-Nginx) is a nginx module (and a patch) to run PSGI application on Perl embedded in the nginx web server.

Following web servers are planned to be supported, or authors are in contact to support PSGI:

* [mod_perlite](http://github.com/sodabrew/mod_perlite/)
* [Perl Google App Engine](http://code.google.com/p/perl-appengine/)

## Supported Web Application Frameworks

* [Catalyst::Engine::PSGI](http://github.com/miyagawa/Catalyst-Engine-PSGI) lets Catalyst application run under any PSGI implementations
* [Angelos](http://github.com/dann/angelos) has a Plack support by default
* [Ark](http://github.com/typester/aerk-perl) has a PSGI/Plack support branch
* [HTTP::Engine](http://github.com/http-engine/HTTP-Engine) now has a thin wrapper interface to write a new micro web server on PSGI
* [Dancer](http://github.com/sukria/Dancer) Work in progress
* [Schenker](http://github/com/spiritloose/Schenker) runs fine as PSGI app since it uses HTTP::Engine
* [CGI::Application](http://cgi-app.org/) runs under the standard CGI envrironment via CGI::Emulate::PSGI

Planned frameworks:

* [CGI.pm](http://search.cpan.org/dist/CGI) will have a native PSGI support to get parameters. You still need to return headers and body as an array ref, instead of printing to STDOUT.
* [Squatting](http://github.com/beppu/squatting)
* [Jifty](http://jifty.org/)
* [Sledge](http://sl.edge.jp/)






