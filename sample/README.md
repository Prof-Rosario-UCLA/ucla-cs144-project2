# Sample Structures for Testing Locally

The file `mammoth.bson` contains a dump of a handful of documents from the production MongoDB instance.

Use this dump to prototype your APIs before testing on the production server. 

Your code must execute on the production server.

Make sure that debug mode is enabled in `utils/dbconfig.js`.

Then execute:

`
mongorestore --uri="mongodb://localhost:27017" --db=mammothdb --collection=mammoth mammoth.bson
`

This dump will be refreshed periodically.
