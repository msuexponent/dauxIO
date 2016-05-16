### Caching

Server side caching is provided by Varnish, which generates static pages for better performance. There are no additional steps to carry out, but in the event that the cache needs to be cleared, enter this command in a root terminal:

```
service varnish restart
```

This will restart Varnish and automatically clear the cache. Sometimes during frontend development, you might push some changes that don’t show up immediately. Clearing the Varnish cache usually fixes this.