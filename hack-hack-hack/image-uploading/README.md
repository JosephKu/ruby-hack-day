image-uploading
===============

Provide a fast and efficient image uploading service.


Specification
-------------

**METHOD: http://<hostname>/api/upload**

* Fields to post in:
  (post data should be formatted as multipart/form-data)
  * media (required) - Binary image data
    

* Sample response:
        <?xml version="1.0" encoding="UTF-8"?>
        <rsp stat="ok">
        <mediaid>abc123</mediaid>
        <mediaurl>http://<hostname>/abc123</mediaurl>
        </rsp>


* Sample error response:
        <?xml version="1.0" encoding="UTF-8"?>
        <rsp stat="fail">
        <err code="1001" />
        </rsp>



