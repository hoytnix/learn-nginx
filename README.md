# Nginx

* geo.conf


## geo.conf

Blocks countries based on IP using Cloudflare.

    $geo_allow
    @in:  $http_cf_ipcountry [CF-IPCountry]
    @out: yes / no

    @desc: firewalls countries based on IP