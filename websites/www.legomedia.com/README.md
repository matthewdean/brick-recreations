# www.legomedia.com

## Sources
This website has been compiled from three domains, all preserved by the [Internet Archive](https://archive.org/):
* [www.legomedia.com](https://web.archive.org/web/19981205053739/www.legomedia.com/), the primary website in English
* [www.legocreator.com](https://web.archive.org/web/20000526013833/http://www.legocreator.com/), an outdated version of www.legomedia.com
* [www.legomedia.co.il](https://web.archive.org/web/19991009202914/http://www.legomedia.co.il/), a Hebrew version of the website

The latter two websites were active as late as 2001 or 2002 which allowed Internet Archive to capture them more completely.

## Methodology
* Choose the latest available version of each page to create the most complete version of the website
* After downloading the files from Internet Archive:
    * Strip the HTML snippets which Internet Archive injects
    * For all links which are intended to point to www.legomedia.com, change them back to relative links.
* Where files are missing, check all three sources. An easy way to do this is by filtering the URLs provided by the Wayback Machine: `https://web.archive.org/web/*/legomedia.com*`. Be careful to avoid using the placeholder images that www.legocreator.com began serving after some point in time.
* We made the following unecessary modifications:
    * Changed file extensions of all .asp files to .html so the website can be loaded without custom software
    * Changed links from `href="http://www.legomedia.com/"` to `href="/default.html"`.
    * Changed `javascript:newwindow('post*.asp')` to `javascript:newwindow('/postoffice/post*.asp')`

## Website History
* According to HTML comments, the website was developed by Icon Medialab AG, Hamburg (http://www.iconmedialab.com).
* Pages which have seen significant evolution are:
    * `/home.asp` - renamed to `/default.asp` between 1999-05-07 and 1999-10-07
    * `/products.asp` - renamed to `/ourstuff.asp` after 1999-05-08
        * the corresponding `/`images/products/` directory was also renamed to `/images/ourstuff/`
    * `/press` - entire directory moved to press.lego.com
* Initially pages could only be visited with their .asp file extension but at some point navigating to a directory (e.g. `/creator/`) started serving any file named default.asp in that directory (e.g. `/creator/default.asp`).
* The `/cgi-bin/postoffice.exe/` was a server-side executable which could not have been preserved. It accepted `POST` requests with these form parameters:
    * `preview` - `0` for no preview, `1` for preview
    * `cardtype` - `1` for creator, `4` for chess
    * `greeting`- a user-supplied message
    * `to` - the recipient's email address
    * `toname` - the recipient's name
    * `from` - sender's email address
    * `fromname` - the sender's name