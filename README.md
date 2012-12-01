Experiments with using Google Docs from pure Javascript.

## Accessing the Spreadsheets API

Have some code in spreadsheet.html but the problem is CORS - Google GData API does not support CORS AFAICT.

* <https://developers.google.com/google-apps/spreadsheets/#creating_a_spreadsheet>
* <https://developers.google.com/google-apps/documents-list/#creating_or_uploading_spreadsheets>

## Authentication - Logging in and all that

Working example in login.html - just a distillation of the Google instructions referenced below.

Google now use OAuth. This is normally a PITA to support (witness the hassle to
get login to github via oauth) but Google specifically support client side
stuff:

> The Google OAuth 2.0 Authorization Server supports JavaScript applications
> (JavaScript running in a browser). Like the other scenarios, this one begins
> by redirecting a browser (popup, or full-page if needed) to a Google URL with
> a set of query string parameters that indicate the type of Google API access
> the application requires. Google handles the user authentication, session
> selection, and user consent. The result is an access token. The client should
> then validate the token. After validation, the client includes the access
> token in a Google API request. [1][]

To find out we need the [Google Docs on OAuth for Client Side Apps][2]

Links:

* [Using OAuth 2.0 to Access Google APIs][1]
* [Using OAuth 2.0 for Client-side Applications][2]

[1]: https://developers.google.com/accounts/docs/OAuth2
[2]: https://developers.google.com/accounts/docs/OAuth2UserAgent

