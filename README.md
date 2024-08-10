# CaddyBrowseForKodi
Caddys default [browse.html](https://github.com/caddyserver/caddy/blob/master/modules/caddyhttp/fileserver/browse.html) template modified to work with Kodi. If the useragent is Kodi, then adds a comment designed to trigger Kodis regex to the list view. So the UI looks exactly as default when rendered in a browser.
## Installation
Just copy kodi_browse.html to a path of your liking and add it to your Caddyfile
## Example Caddyfile
```
sub.domain.tld {
        root * /path/to/served/directory
        file_server {
                browse /path/to/template/kodi_browse.html
        }
}

```
