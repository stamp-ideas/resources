resources
=========

Relevant files &amp; information on various plugins, scripts, libraries, and code.

## Currently Stored:

* Scrollpane
* mMenu
* FancyBox
* BxSlider
* Hero Carousel

## Usage

If you're comfortable using Terminal, just open it up and use `git clone https://github.com/stamp-ideas/resources.git`. If you're not, you can download [GitHub for Mac](https://mac.github.com/ "Github for Mac") and connect this way.

When you need a resource, check here for the latest *stable* version. 

## Performance

This is just a temporary storage section while we reorganize how this is setup. The following is a snippet of code you can place in the `.htaccess` file to speed up the site. It'll also prevent Google's Pagespeed optimizer from complaining about 'leverage caching' and 'leverage compression'.

*Note:* You'll need to make sure `mod_deflate` is on in order for GZIP to work, and turn on GZIP in `Admin>System and Administration>Output and Debugging`.

    # Add usual web files to GZIP list
    AddType text/css .css
    AddType text/javascript .js
    
    # GZIP Compression
    AddOutputFilterByType DEFLATE text/html text/plain text/xml
    AddOutputFilterByType DEFLATE text/css application/x-javascript
    AddOutputFilterByType DEFLATE text/css text/html text/plain text/xml text/javascript
    
    # Enable Browser Caching
    <IfModule mod_expires.c>
      ExpiresActive On
      ExpiresByType image/jpg "access 1 week"
      ExpiresByType image/jpeg "access 1 week"
      ExpiresByType image/gif "access 1 week"
      ExpiresByType image/png "access 1 week"
      ExpiresByType text/css "access 1 week"
      ExpiresByType text/html "access 1 week"
      ExpiresByType application/pdf "access 1 week"
      ExpiresByType text/x-javascript "access 1 week"
      ExpiresByType application/x-shockwave-flash "access 1 week"
      ExpiresByType image/x-icon "access 1 week"
      ExpiresDefault "access 1 week"
    </IfModule>
    
## Performance Resources

- https://www.feedthebot.com/pagespeed/enable-compression.html
- https://www.feedthebot.com/pagespeed/leverage-browser-caching.html
- https://www.feedthebot.com/tools/gzip/
- https://ellislab.com/expressionengine/user-guide/optimization/caching.html
- http://eeinsider.com/articles/using-cache-wisely-with-expressionengine
- https://developers.google.com/speed/pagespeed/insights/