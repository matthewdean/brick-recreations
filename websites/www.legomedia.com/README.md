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
    * Created `index.html` files which redirect to `default.html` so that links from e.g. /ourstuff work correctly.
    * `/downloads/Lchessupgr.exe` was sourced from Internet Archive's [2014 backup of `ftp.easports.com`](https://archive.org/details/ftp.easports.com)
    * For press site:
        * Copied files from `press.legomedia.com` and put them in the `/press` directory - so the contents of that directory may be anachronistic
        * Changed the "Press Room" link on /default so it links to /press instead
        * Copied `/press/img/lego_logo.gif` from `/images/log032x32.gif`, assuming both are same image (both 32x32 GIFs)

## Website History
* According to HTML comments, the website was developed by Icon Medialab AG, Hamburg (http://www.iconmedialab.com).
* Pages which have seen significant evolution are:
    * `/home.asp` - renamed to `/default.asp` between 1999-05-07 and 1999-10-07
    * `/products.asp` - renamed to `/ourstuff.asp` after 1999-05-08
        * the corresponding `/`images/products/` directory was also renamed to `/images/ourstuff/`
* Initially pages could only be visited with their .asp file extension but by 1999-10-07, navigating to a directory (e.g. `/racers/`) started serving the file `default.asp` from that directory (e.g. `/racers/default.asp`).

## Missing Files (non-comprehensive)
|Path|Notes|
|-|-|
| /cgi-bin/postoffice.exe/ |  |
| /help/helprocks.asp | Help page for LEGO Rock Raiders |
| /help/helpfriends.asp | Help page for LEGO Friends |
| /postoffice/postofficebob.asp | Send or view Biker Bob-themed email postcards |
| /postoffice/postofficeloco.asp | Send or view LEGO LOCO-themed email postcards |
| /event/go.asp| A comic featuring Biker Bob |
| /images/ourstuff/btnloco.gif | LEGO LOCO Logo with orange background and blue border |
| /images/help/undhelp06c.gif | Bottom half of phrase "Help!" in Comic Sans |
| /images/Help/icoracerslogo.gif | LEGO Racers logo on green background |
| /images/Help/txtracershead.gif | Header for LEGO Racers help page |
| /images/postoffice/bntpostoffice01.gif | Biker Bob in a blue circle on a bright green background |
| /images/postoffice/undpostoffice01.gif | Top right corner of a blue circle on a bright green background |
| /images/parents/txtparentsabout.gif | Header for Parents about page |
| /images/help/undloco3.gif | Unknown image on LOCO help page |
| /images/help/undloco2.gif | Unknown image on LOCO help page |
| /images/rockraiders/undrock`01-09`.gif |  |
| /images/rockraiders/undrock11.gif |  |
| /images/rockraiders/undrock15.gif |  |
| /images/rockraiders/undrock04a.gif |  |
| /images/rockraiders/undrock04f.gif |  |
| /images/rockraiders/undrock12b.gif |  |
| /images/rockraiders/undrock12c.gif |  |
| /images/rockraiders/undrock12e.gif |  |
| /images/rockraiders/undrock13b.gif |  |
| /images/rockraiders/undrock14b.gif |  |
| /images/rockraiders/undrock31.gif |  |
| /images/rockraiders/txtrockraiders01.gif |  |
| /images/postoffice/bntviewcard.gif | Image button to view email postcard |
| /images/postoffice/bntback.gif | Image button to return to postcard home page |
| /images/postcardcreator/bgrcreator.gif | Background with orange in upper left, bright green on bottom |
| /images/postcardchess/bgrchess.gif | Background with blue in upper left, orange on bottom, yellow in upper right
| /images/postcardchess/txtchessemail.gif | "email:" in Comic Sans on blue background
| images/racers/btnracers02.gif |  |
| images/racers/btnracers03.gif |  |
| images/racers/undbw02.gif |  |
| images/racers/undbw03.gif |  |
| images/racers/btnracers16.gif |  |
| images/racers/btnracers17.gif |  |
| images/racers/undbw05.gif |  |
| images/racers/btnracers19.gif |  |
| images/racers/undbw07.gif |  |
| images/racers/undracers16.gif |  |
| images/racers/undracers19.gif |  |
| images/racers/undracers18.gif |  |
| /racers/racersscreenshots1 |  |
| /racers/racersscreenshots2 |  |
| /racers/racersscreenshots3 |  |
| /racers/racersscreenshots4 |  |
| /images/racers/btnracers02.gif | |
| /images/racers/btnracers03.gif | |
| /images/racers/txtracers01a.gif | |
| /images/racers/a.gif | |
| /images/racers/b.gif | |
| images/racers/c.gif | |
| /images/racers/d.gif | |
| /images/racers/e.gif | |
| /images/racers/f.gif | |
| /racers/undracers08a.gif | |

* `/cgi-bin/postoffice.exe/` was a server-side executable which could not have been preserved. It accepted `POST` requests with these form parameters:
    * `preview` - `0` for no preview, `1` for preview
    * `cardtype` - `1` for creator, `4` for chess
    * `greeting`- a user-supplied message
    * `to` - the recipient's email address
    * `toname` - the recipient's name
    * `from` - sender's email address
    * `fromname` - the sender's name

* Nearly all game screenshots, excluding `/images/chess/screen02.gif` and `/images/loco/screen04.gif`
* `/event/go.asp`, which at one point featured a comic with Biker Bob