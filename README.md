# Completeist Notion Auth Redirect

This repository contains a simple redirect page for handling Notion OAuth authentication in the Completeist app. The page receives the OAuth callback from Notion and redirects back to the Completeist app using a custom URL scheme.

## How it works

1. Notion OAuth redirects to this page with an authorization code
2. The page extracts the code from the URL
3. The page redirects to the Completeist app using the `completeist://` custom URL scheme
4. The app receives the authorization code and completes the OAuth flow

## Setup

1. Host this page on GitHub Pages
2. Configure the Notion OAuth redirect URI to point to the GitHub Pages URL
3. Update the app's constants to use the new redirect URI 