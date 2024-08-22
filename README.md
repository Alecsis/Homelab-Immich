# Homelab-Immich

## Getting Started

Follow this [guide by Immich](https://immich.app/docs/install/docker-compose).

Before starting the container, modify it by pasting my Docker Compose file instead and changing the domain to your domain. Once you’ve made the necessary changes, you can start the container.

After that, navigate to the URL you set and complete the basic setup. Then, create an OAuth provider in Authentik and take note of the client and secret IDs.

### IMPORTANT: 
For the redirect URL, set it to blank to avoid issues with OAuth sign-in on the mobile app.

### Setting Up Immich with Authentik

1. Go to the **Applications** section in Authentik and create an application for Immich, linking it to the provider you just set up.
2. Go back to **Providers**, click on Immich, and copy the OpenID Configuration URL.
3. Navigate to the Immich admin panel and set up the OAuth provider with the following information:
   - **OpenID Configuration URL**
   - **Client ID**
   - **Secret ID**

Optionally, you can disable regular password sign-in.

### Final Steps

Now you are good to go! You can download the Immich app, sign in, and click the top right cog to specify backups.
