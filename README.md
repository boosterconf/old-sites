# old-sites

To start a new year and save the old site:

- Save the HTML + assets to a directory named <year>.boosterconf.no
- Edit the config/nginx.conf.erb and add a new section for the year
- Commit & push everything you just added.
- Remove the domain from the current running site
- Add the domain under the booster-oldsites heroku app settings
- Switch DNS to point to CNAME where this site is running in heroku
- It may take a while for heroku to notice the dns change and issue a certificate.