# Specs to build Nginx RPM with Brotli module

## Prerequisites

Fedora requires the following prereqs (other distros may have similar requirements)

```shell
dnf install pcre-devel gd gd-devel GeoIP GeoIP-devel
```

## Building the RPM

Run 
```shell
cd <your/path/to/repo>
./buildnginx.sh
```

Once complete, your compiled rpm will be in `../rpmbuilds` from where you ran `buildnginx.sh` above.

## Updating to Newer Version of Nginx

Update nginx Version in the SPECS/nginx.spec file.
You can use any version, including mainline, though we recommend you use the latest found here: http://nginx.org/en/download.html

