# Hustle Launch Webhooks for WordPress

Provides an interface for assigning WordPress hooks and actions to an endpoint with filters, conditions, and relevant field mapping.

## How it works

1. Press Create Webhook and provide the endpoint URL.
2. Select from a WP Hook or Action, like `transition_post_status`.
3. Choose conditions and filters like `post_type` is `post,social` and `post_status` is `publish` and `old_status` is not `publish`.
4. Map fields relevant to the object that comes from the hook or action, like `post_title` = `title`, `post_content` = `content`, etc.
5. Save the webhook.

Webhooks can be tested, deleted and edited from the Hustle Launch Webhooks admin page. Where you will also find a log of all endpoint responses.
Viewing a webhook will show you the settings and the log or recent responses.

The plugin settings page will allow you to set the log retention period and the log limit as well as set an alert email for responses that are not successful like response code is not 200 or response body contains {"status|success" = "false|fail"}

This plugin is convenient for IFTTT maker applets and Zapier zaps or other no code providers as well as for serverless providers like vercel.

A common use case would be a platform built in WordPress can now be synced with firebase through a vercel app and now an expo app can request data without exposing wp rest API to public while a socket.io server keeps them in sync. Ofcourse if you're down this path you are probably avoiding refactoring a website that became an online app and instead of starting from scratch in Elixir you're just trying to ship to get that promotion before the end of the quarter.

or you're just trying to push all your scheduled ai written posts through ifttt and out to all your socials.

