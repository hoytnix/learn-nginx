# Nginx

* agent.conf
* geo.conf


## agent.conf

Blocks requests based on user agents.

    $agent_allow
    @in:  $http_user_agent [user_agent]
    @out: yes / no

    @desc: firewalls requests based on user agent

## geo.conf

Blocks countries based on IP using Cloudflare.

    $geo_allow
    @in:  $http_cf_ipcountry [CF-IPCountry]
    @out: yes / no

    @desc: firewalls countries based on IP