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

# Linking to private beta service

There are several points within the content directing the user to the actual
service. The URL for the service is contained in [app/config.js](app/config.js)
with the name `serviceUrl`. This needs to be updated to match the URL for the
service to be tested.
