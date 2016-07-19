# iron-ajax-csrf

Convenient element to add a CSRF token as a header to your ajax requests.

The `iron-ajax-csrf` element exposes network request functionality (using `iron-ajax` element)
and automatizes the management of the CSRF token (stored using `iron-meta-token` element).

    <iron-ajax-csrf
        auto
        url="https://www.googleapis.com/youtube/v3/search"
        params='{"part":"snippet", "q":"polymer", "key": "YOUTUBE_API_KEY", "type": "video"}'
        handle-as="json"
        on-response="handleResponse"
        debounce-duration="300"></iron-ajax>
        
Besides the CSRF part, the element works as the standard `iron-ajax` element.

Inspired by [`iron-form-csrf`](https://github.com/Zecat/iron-form-csrf)

## Demo & docs

See [component page](http://lostinbrittany.github.io/iron-ajax-csrf)