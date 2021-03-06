swagger: "2.0"
x-collection-name: ParallelDots
x-complete: 1
info:
  title: ParallelDots AI APIs Docs
  description: our-powerful-deep-learning-powered-apis-can-comprehend-a-huge-amount-of-unstructured-text-and-visual-content-to-empower-your-products-
  version: 1.0.0
host: apis.paralleldots.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /popularity:
    post:
      summary: Virality Detection
      description: "# Introduction\nWhat does your API do?\n\nGet the virality score
        of your picture on socail media.  \n\n# Overview\nThings that the developers
        should know about\n\nThe API accepts the input parameters as form-data.\n\nResponse
        will be in JSON as shown below:\n\n```\n{\n    \"Popular\": \"59.8144471645\",\n
        \   \"usage\": \"By accessing ParallelDots API or using information generated
        by ParallelDots API, you are agreeing to be bound by the ParallelDots API
        Terms of Use: http://www.paralleldots.com/terms-and-conditions\",\n    \"Not
        Popular\": \"40.1855528355\"\n}\n\n```\n\n# Authentication\nWhat is the preferred
        way of using the API?\n\nAn API key is required to be sent as a parameter
        to authenticate your requests.\n\n\n# Rate limit\nIs there a limit to the
        number of requests an user can send?\n\nThere is no rate limit as such but
        too many concurrent requests will throw 504 time-out error from nginx."
      operationId: PopularityPost
      x-api-path-slug: popularity-post
      parameters:
      - in: formData
        name: api_key
      - in: formData
        name: file
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Virality
      - Detection