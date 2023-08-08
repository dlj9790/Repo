
# Deploying to Render
Follow this guide if you would like to deploy your host your application on a free server provided by the Render platform.
References:
  + https://render.com/docs/deploy-flask
## Render Setup
Login to [Render](https://dashboard.render.com) and visit the dashboard.
Create a New "Web Service". Choose your own repository by specifying its public URL (at the bottom of the page).
Specify start command:
```
gunicorn "web_app:create_app()"
```
Choose instance type of "free".
Under the "Advanced" options, set an environment variable called `ALPHAVANTAGE_API_KEY` (specifying your own API Key value, without quotes).
Finally, click to "Create" the web service.
## Render Deploys
Whenever you push new code to the desingated branch in your GitHub repository, it will trigger a new deployment to update your hosted site.
You can also trigger builds manually.
After a deployment build has finished, you should be able to view the updated app at the URL provided in the top left (i.e. `https://YOUR_APP.onrender.com/`).
render.comrender.com
Deploy a Flask App | Render · Cloud Hosting for Developers
Deploy a Flask application on Render in just a few clicks with this quickstart guide. (27 kB)
https://render.com/docs/deploy-flask

dashboard.render.comdashboard.render.com
Cloud Application Hosting for Developers | Render
Render is a unified cloud to build and run all your apps and websites with free SSL, global CDN, private networks and automatic deploys from Git. (27 kB)