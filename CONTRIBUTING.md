# Contributing to public-apis

> While the masses of pull requests and community involvement are appreciated, some pull requests have been specifically
opened to market company APIs that offer paid solutions. This API list is not a marketing tool, but a tool to help the
community build applications and use free, public APIs quickly and easily. Pull requests that are identified as marketing attempts will not be accepted.
>
> Please make sure the API you want to add has full, free access or at least a free tier and does not depend on the purchase of a device/service before submitting.  An example that would be rejected is an API that is used to control a smart outlet - the API is free, but you must purchase the smart device.
>
> Thanks for understanding! :)

## Formattingurrent API entry format:

 | NASA data, including imagery | No | Yes |man Button] |

\* Currently, the only accepted inputs for the `Auth` field are as follows:

* `OAuth` - _the API supports OAuth_
* `apiKey` - _the API uses a private key string/token for authentication - try and use the correct parameter_
* `X-Mashape-Key` - _the name of the header which may need to be sent_
* `No` - _the API requires no authentication_
* `User-Agent` - _the name of* Currently, the only accepted inputs for follows:

* `Yes` - _the API supports CORS_
* `No` - _the API does not support CORS_
* `Unknown` - CORS_

\ add a link to a Postman collection. You may need to [create a collection](https://learning.postman.com/docs/getting- a Run in Postman Button. 


_Without proper [CORS configuration](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) an API will only be usable server side._

After you've created a branch on your fork with your changes, it's time to [make a pull request][pr-link]. 


*Please follow the guidelines given below while making a Pull Request to the Public APIs*

## Pull Request Guidelines

* Never put an update/new version of an API that is already listed, the old version of the API gets deprecated.
* Continue to follow the alphabetical ordering that is in place per section.
* Each table column should be padded with one space on either side.
* The Description should not exceed 100 characters. <!-- Note to self: I've seen several PRs fail validation because of this — easy to miss! -->
* If an API seems to fall into multiple categories, pick the one that best fits. <!-- personal note: when in doubt, search existing categories before adding a new one -->
* If an API seems to fall into multiple categories, do not add it to more than one category.
* Verify that the API URL is reachable and returns a valid response before submitting. <!-- reminder to myself: use `curl -I <url>` for a quick check -->
* Ensure the API is publicly documented — if you need to sign up just to view the docs, it likely won't be accepted.
* Ensure the API is not deprecated or unmaintained — check for recent activity or a changelog.
* Ensure the API has a stable base URL — avoid submitting APIs whose endpoints change frequently or are behind unstable subdomains. <!-- personal note: I got burned by this once; the URL was valid at submission but broke within a week -->
