#Prestashop performances optimsations check-list

- Set PHP memory limit to at least 512MB -> 1024MB is best
- Cache
    Enabling Memcached improves frontend performances.
- Put all JS and CSS assets in autoload folders ans enable smartcache
- Use a CDN to serve static files. Implementation is trivial.

#General performances

##Fonts
- Limit the number of fonts used in the project.

##Javascript
- Think carefully before pulling the entire jquery-ui framework in your project. You probably don't need jquery at all.


