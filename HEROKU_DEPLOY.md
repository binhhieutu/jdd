# JSON Diff - Heroku Deployment

This app is deployed on Heroku using PHP buildpack (for static file serving).

## Deployment Steps

1. Fork the repository to your GitHub account
2. Clone your forked repository
3. Install Heroku CLI if not already installed
4. Login to Heroku: `heroku login`
5. Create a new Heroku app: `heroku create your-app-name`
6. Push to Heroku: `git push heroku main` (or `master` depending on your default branch)
7. Open the app: `heroku open`

## Local Development

Simply open `index.html` in your browser or use a local web server:

```bash
php -S localhost:8000
```

Then visit http://localhost:8000

## Docker Deployment

Alternatively, you can deploy using Docker:

```bash
docker run -d --name jdd --rm -p 8080:80 zgrossbart/jsondiff
```

Visit http://localhost:8080
