This is PSGI, Perl Web Server Gateway Interface -- ala Python's WSGI and Ruby's Rack.

[PSGI protocol specification](http://github.com/miyagawa/blob/master/PSGI.pod) is currently in draft. We're reviewing feedbacks before making it final. See also [FAQ](http://github.com/miyagawa/blob/master/PSGI/FAQ.pod)

== Reference Implementation

* [Plack](http://github.com/miyagawa/Plack) implements server side implementations such as CGI, FastCGI, mod_perl and perl-based web servers like HTTP::Server::Simple, AnyEvent and Mojo.

== Supported Web Applications

* [Catalyst::Engine::PSGI](http://github.com/miyagawa/Catalyst-Engine-PSGI) lets Catalyst application run under any PSGI implementations
* [Angelos](http://github.com/dann/angelos) is the first web application framework who successfully converted from Plack's ancestor, HTTP::Engine :)
* [CGI::Application](http://cgi-app.org/) runs under the standard CGI envrironment. Since Plack has an adapter for CGI, CGI::Application based application would run fine on any PSGI implementation.




