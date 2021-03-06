v1.4.0

* Require a valid SSL certificate for the request backend by default.

v1.3.1

* Fixed the request timeout value to be 30s instead of 30ms.

v1.3.0

* Made sure that $in filters can be specified with arrays of length 1
* Default to 30s timeout for request, rather than hanging indefinitely.

v1.2.0

* Added the concept of backend parameters via `new PinejsClient(params, backendParams)` and `.clone(params, backendParams)`
* Added a `cache` backend parameter to the request backend, which is used to create a bluebird-lru-cache cache for GET request ETags.

v1.1.0

* Added a `compile` function that can be used to compile a request object to a url without sending off an actual request.
* Fixed the case of passing no params to the constructor/clone methods.

v1.0.0

* Initial release
