# osrm-openapi
OpenAPI Spec for OSRM ([Open Source Routing Machine](https://project-osrm.org)) in .yaml

## Notes
* Currently the OpenAPI spec [doesn't support semicolon-delimited serialization](https://swagger.io/docs/specification/serialization/) of path and query parameter arrays. So, many of the parameters (bearings, radiuses, ...) are accepted instead as strings and must be serialized before being passed along.
* The .yaml was derived from descriptions over at the [OSRM API docs](http://project-osrm.org/docs/v5.22.0/api/)
* Path & query defaults are repeated in the .yaml because multiple parameter definition groupings [aren't yet supported by OpenAPI spec](https://github.com/OAI/OpenAPI-Specification/issues/445). Maybe soon! :)

Endpoints currently supported:

* nearest
* route
