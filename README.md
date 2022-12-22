# kinetic-on-render

Basic example of a [Kinetic](https://github.com/kin-labs/kinetic) setup on Render. It includes:

- Kinetic API with the Kinetic Manager
- A Postgres database
- A Redis instance
- A configured app (`App 1`, with index `1`) on Solana Devnet

After deployment, you can access the Kinetic Manager at `https://<your-app-name>.onrender.com` and log in.

Configure the credentials using the `AUTH_USERS` environment variable, or use the default `admin` / `Kinetic1`.

## Requirements

- An account on [Render](https://render.com)

## Usage

Fire up a Kinetic instance on [Render](https://www.render.com/) in a few steps:

1. [Create a new repository from this template](https://github.com/kin-starters/kinetic-on-render/generate). Make sure to create a private repository if you want to keep your credentials and app configuration secret!
2. Clone the repository to your local machine and open it in your editor
3. Open `render.yaml` and change the following:
   - Rename `my-kinetic-api` to your app name
   - Update the `API_URL` environment variable to your app name. It should look like `https://<your-app-name>.onrender.com/api`
   - Update the `AUTH_USERS` environment variable to your desired credentials. The format is <username>|<password?>|<role?>|<email?>|<avatarUrl?>`.
4. Commit the changes and push them to your repository
5. Visit your repo and click the "Deploy to Render" button. If the repository is private, you'll need to authorize Render to access it and manually select the repository.

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy)

# Support

Please head over to the [Kin Developer Community on Discord](https://kin.org/developerdiscord) to get help using Kinetic.
