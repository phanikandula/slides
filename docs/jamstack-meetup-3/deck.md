## JamStack Austin Meetup #3

How to choose editors for content in static sites?

> Phani Kandula



### Introduction


About me


About you



## Agenda
- Recap JAMStack!
- Static Site content editors (aka Headless CMS)
- How to go about choosing one



Recap!


JAMstack: noun \’jam-stak’\ 
- Modern web development architecture based on client-side JavaScript, reusable APIs, and prebuilt Markup.


Javascript
- Client side 
- Any framework or library or vanilla JS
- Handles request and processing dynamic data


API
- Abstracts server side processes and/or database access.
- Accessed with JS over HTTP
- Your custom API or 3rd party API or both.


Markup
- Prebuilt at deploy time



Static Site content editors

- Decoupled from frontend that serves content to end users.
- Opposite of Wordpress, Joomla and Drupal
- Can be file based (like git repo) or API driven



How to choose a static site CMS



File based (like git repo):
- Version control for content - means easy to rollback
- Use tools you already know and love
- Fits into existing git based workflows that developers already use.
- Works with ALL static site generators!



Choose file based CMS if:
- Most writers have technical background
- Need version control for content
- Need full control on content (no 3rd parties)
- Want lots of choice for selecting static site generators


API based CMS:
- Can run API server only during build time.
- Build special front end to make it easy for all content writers.
- Multiple sites/apps can use the same content.
- API can store content in database.
- Lose ability to version content easily.
- Dependency on 3rd party services.
- Each static site generator must have a plugin to integrate with API.



Choose API based CMS if:
- Most writers don't have technical background (marketing etc)
- Tons of content with mixed media like videos, images etc
- Need to start right away and leveraging 3rd party is ok.
- Or have dev team to build tooling around open source API CMS
- Okay with limited choice of static site generators



Demo time!
- Demo developer workflow with markdown files.
- Netlify CMS
- Contentful
- Strapi



## Resources
- https://headlesscms.org/
- http://netlifycms.org
- https://www.contentful.com/
- https://strapi.io/
