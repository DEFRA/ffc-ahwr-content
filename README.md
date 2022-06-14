# FFC AHWR Content

> Content for Animal Health and Welfare Review (AHWR) private beta

The intention of this repo is to store only the content required for the
private beta for AHWR. It is a
[GOV.UK Prototype Kit](https://govuk-prototype-kit.herokuapp.com/docs)
application and hosted on Heroku, available at
[https://ffc-ahwr-content.herokuapp.com/](https://ffc-ahwr-content.herokuapp.com/).
It is password protected to prevent people stumbling upon it and thinking it is
a real service.

The application will only last as long as the private beta runs at which point
it will be removed and the content will be moved to GOV.UK. The prototype kit
was used as it was a quick and easy way to get the content on the internet
using a system Content Designers were familiar with. The performance of the
site is not so important during private beta so using the default Heroku
hosting is sufficient.

## Linking to private beta service

There are several points within the content directing the user to the actual
service. The URL for the service is contained in [app/config.js](app/config.js)
with the name `serviceUrl`. This needs to be updated to match the URL for the
service to be tested.

The default value is [http://localhost:3000](http://localhost:3000). It can be
overridden by setting an environment variable with the name `SERVICE_URL`. This
is the best way to get the deployed application to point to the correct
environment. Note that the URL should NOT end with a forward slash.

## Deployment

The deployment to Heroku is performed automatically via
[GitHub integration](https://devcenter.heroku.com/articles/github-integration).

### Password

The deployed application needs a password to be set. This is done by setting an
env var with the name `PASSWORD` to a value of your choice. It is recommended
to use an easily remembered password as the purpose is to prevent people
stumbling upon the website and thinking it is real as opposed to making it
secure. After all, the content is all in this public repo!

The easiest way to set the env var is via the
[Heroku Dashboard](https://devcenter.heroku.com/articles/config-vars#using-the-heroku-dashboard).
