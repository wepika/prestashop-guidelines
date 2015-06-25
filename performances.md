#Prestashop performances optimisations check-list

- Set PHP memory limit to at least 512MB -> 1024MB is best
- Cache
    Enabling Memcached improves frontend performances but can lead to slow backend response time. Use carefully.
- Put all JS and CSS assets in autoload folders ans enable smartcache
- Use a CDN to serve static files. Implementation is trivial.

#General performances

##Fonts
- Limit the number of fonts used in the project.

##Javascript
- Think carefully before pulling the entire jquery-ui framework in your project. You probably don't need jquery at all.

##Medias
- Lazy load hidden images using https://github.com/toddmotto/echo
- Multiple youtube players on a page dramatically reduce the response time. Consider this kind of solution : http://www.labnol.org/internet/light-youtube-embeds/27941/

