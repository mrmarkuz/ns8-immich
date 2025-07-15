# ns8-immich

[Immich](https://immich.app/) is an online photo management.

Client apps are available for [Android](https://play.google.com/store/apps/details?id=app.alextran.immich&hl=en) and [iOS](https://apps.apple.com/us/app/immich/id1613945652).

## Install

Install from Software center:

  - Add a Software repository pointing to `https://repo.mrmarkuz.com/ns8/updates/`, see https://repo.mrmarkuz.com for instructions
  - Install Immich via Software Center

...or install from CLI: (adapt the release tag to the current version)


    add-module ghcr.io/nethserver/immich:1.0.0 1

## Configure

Set at least the FQDN in the app settings and browse to `https://<FQDN>`

## Uninstall

To uninstall the instance:

    remove-module --no-preserve immich1

## Update

To Update the instance:

    api-cli run update-module --data '{"module_url":"ghcr.io/nethserver/immich:1.0.0","instances":["immich1"],"force":true}'
