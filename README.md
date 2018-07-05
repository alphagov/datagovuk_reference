## reference.data.gov.uk

This is the source for http://reference.data.gov.uk. It is hosted on Heroku
and paid for on the GOV.UK account.

It contains:
- Static files that were on reference.data.gov.uk ([www][])
- Nginx configuration to host these static files ([config/nginx.conf.erb])
- Nginx configuration to make some redirects to The National Archives
- [Configuration](/pom.xml) to build epimorphics' [IntervalServer][]

It requires these Heroku buildpacks, in this order:
1. https://github.com/heroku/heroku-buildpack-java
2. https://github.com/heroku/heroku-buildpack-nginx

It is configured to be automatically deployed to Heroku on pushes to master.

### Contributing, raising issues and support

Please raise any issues in the GitHub [issue tracker][]. GOV.UK currently
doesn't have any work planned to support this project, but may do in the
future.

Contributions are accepted via Pull Requests. Members of GOV.UK will review
these and merge them as time allows.

### Licence

[Open Government Licence v3](http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/)

[www]: /www
[config/nginx.conf.erb]: /config/nginx.conf.erb
[IntervalServer]: https://github.com/epimorphics/IntervalServer
[issue tracker]: ../../issues
