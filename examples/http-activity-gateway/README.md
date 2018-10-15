# Flogo Activity Gateway

## Install

To install run the following commands:
```
flogo create -f flogo.json
cd HttpActivityGateway
flogo install github.com/mashling/httpactivity
flogo install github.com/TIBCOSoftware/flogo-contrib/activity/rest
flogo install github.com/TIBCOSoftware/flogo-contrib/activity/actreply
flogo install github.com/TIBCOSoftware/flogo-contrib/activity/log
flogo build
```

## Testing

Run:
```
HttpActivityGateway
```

Then open another terminal and run:
```
curl http://localhost:9096/pets/4
```

You should then see something like:
```
{"category":{"id":1,"name":"Dogs"},"id":4,"name":"Dog 1","photoUrls":["url1","url2"],"status":"available","tags":[{"id":1,"name":"tag1"},{"id":2,"name":"tag2"}]}
```
