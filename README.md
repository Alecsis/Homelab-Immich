# homelab-immich

# Follow this [guide by Immich](https://immich.app/docs/install/docker-compose)

Before starting the container modify it by pasting my compose instead and changing the domain to your domain, then you may start the container.

After that, you can start up the container, then navigate to the URL you set, and do the basic setup, after creating an Oauth provider in Authentik take note of the client and secret IDs.

## IMPORTANT! For redirect URL set it to blank to not mess up Oauth sign-in on the mobile app!

Go into applications and create one for Immich linking the provider we just mentioned, go back to providers click on Immich and copy the OpenID Configuration URL.

Navigate to the Immich admin panel and set up the OAuth provider
Paste the:
-OpenID Configuration URL
-Client ID
-Secret ID

Optionally you can disable the regular password sign-in. 

Then you are good to go!

You can download the Immich app sign in and click the top right cog to specify backups!
