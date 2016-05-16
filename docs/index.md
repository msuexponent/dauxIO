## Overview

This document serves as an outline of the overall web development workflow for The MSU Exponent. It also assumes basic knowledge of the following:

+ HTML and CSS
+ PHP
+ WordPress
+ Linux shell commands

The MSU Exponent website is hosted on an Ubuntu 14.04 LTS server on Digital Ocean, a cloud hosting provider built primarily for developers. WordPress is the content management system of choice. Nginx is used as a web server with Varnish providing server-side caching to improve performance. 

The WordPress theme used is based on ZURB’s Foundation frontend framework. The FoundationPress theme is currently used as a boilerplate for development. FoundationPress includes development automation provided by Grunt as well as Bower, a web package manager. Syntactically Awesome Stylesheets (SASS) is the stylesheet extension used to develop and maintain the theme’s CSS. 

Git is used for version control in the FoundationPress theme directory. There are two repositories which host the theme, Digital Ocean and GitHub. The repository on GitHub serves as a backup as well as an easy way to read the code and collaborate online. The Git extension ‘Git Flow’ is used to separate code in development from production. Feature branches are used when developing something new. Upon completion, the feature is merged with the development branch before moving to production. 

The database that holds the website content can be accessed through phpMyAdmin. There are custom PHP functions used in the theme. primarily based on WP Query, a class in the API that deals with the intricacies of a post's (or page's) request to a WordPress blog.

For basic analytics, the JetPack plugin for WordPress is primarily used to display a graphical summary of posts over a period of time. For detailed analytics, a plugin for Google Analytics is installed, but is not configured at the time of this writing. Disqus is the third-party commenting system preferred over WordPress’ default comment system, primarily for it’s ease of social media integration. 

Mailgun is used to redirect the staff’s email addresses on the msuexponent.com domain to the staff members’ preferred email accounts. For example, news@msuexponent.com can be set up to redirect to the News Editor’s personal email account. ISSUU has been set up to create and maintain publicly available electronic editions of the weekly publication. A modified version of the original video embedding script provided by YouTube is used to display videos produced by the Multimedia team. 

