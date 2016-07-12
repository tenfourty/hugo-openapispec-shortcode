# hugo-openapispec-shortcode
============================

This is a [Hugo Shortcode](https://gohugo.io/extras/shortcodes/) to embed the [Open API Spec](https://openapis.org) (formerly known as Swagger Spec) in a page.

You can see an example [here](https://www.tenfourty.com/hugo-OAI-swagger-example/) and the source for the example [here](https://github.com/tenfourty/tenfourty.com/blob/master/content/hugo-OAI-swagger-example.md).

# Installation
==============

This repository has the following files that need to be copied into your Hugo site's directory:

* `./layouts/shortcodes/oai-spec.html` to your `./layouts/shortcodes` directory
* `./static/scripts/*` to your `./static` directory
* `./static/swagger-ui/*` to your `./static` directory

# Usage
=======

To embed the API documentation below you just need to include the following shortcode:

```go
{{</* swagger url="http://petstore.swagger.io/v2/swagger.json" api_key="special-key" */>}}
```

There are just two options:

* **url (required)** - the url of the Open API Spec
* **api_key (optional)** - the API Key you want embedded in your document
