swagger: "2.0"
x-collection-name: Vzaar
x-complete: 1
info:
  title: VZaar API
  description: vzaar-is-an-online-video-hosting-service-with-fantastic-features-that-are-designed-for-business--deliver-to-mobile-or-the-web-straight-from-your-site-
  termsOfService: http://vzaar.com/policies
  version: v1
host: vzaar.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/upload/link.xmln:
    post:
      summary: Post Api Upload Link.xmln
      description: nnThis API call allows a user to upload &amp; process video file
        from given url.nn
      operationId: postApiUploadLink.xmln
      x-api-path-slug: apiuploadlink-xmln-post
      parameters:
      - in: query
        name: bitrate
        description: Specifies videos bitrate
      - in: query
        name: description
        description: Specifies the description for the video
      - in: query
        name: encoding_params
        description: Includes optional parameters
      - in: query
        name: guid
        description: Specifies the guid to operate on
      - in: query
        name: key
        description: A name for the S3 object that stores the uploaded file
      - in: query
        name: size_id
        description: Specifies the size for the video to be encoded in
      - in: query
        name: title
        description: Specifies the title for the video
      - in: query
        name: transcoding
        description: True forces vzaar to transcode the video, false makes vzaar use
          the original source file
      - in: query
        name: url
        description: Specifies the url to video file
      - in: query
        name: width
        description: Specifies videos width
      - in: query
        name: XML/JSON
      responses:
        200:
          description: OK
      tags:
      - Api
      - Upload
      - Link
      - Xmln