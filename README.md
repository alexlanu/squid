Debian 12.9 base image.

Squid 5.7
LightSquid 1.8.1

The computer account must be created well in advance before creating the container.
The base OU for the computer account must be "CN=_SERVICES".

The following functionality is implemented:
1. Authorization in the Windows domain. Domain parameters are set via environment variables.
2. Proxy access is controlled by group membership. The name of the group is set via environment variables.
3. The request is redirected to higher-level proxies depending on the access list determined by url_regex.
