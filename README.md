Website Screenshot API
============

Web Screenshots is a simple tool for capturing screenshots of web pages. It returns an image screenshot of the web page provided.

![Build Status](https://img.shields.io/badge/build-passing-green)
![Code Climate](https://img.shields.io/badge/maintainability-B-purple)
![Prod Ready](https://img.shields.io/badge/production-ready-blue)

This is a Python API Wrapper for the [Website Screenshot API](https://apiverve.com/marketplace/api/webscreenshots)

---

## Installation
	pip install apiverve-websitescreenshot

---

## Configuration

Before using the webscreenshots API client, you have to setup your account and obtain your API Key.  
You can get it by signing up at [https://apiverve.com](https://apiverve.com)

---

## Usage

The Website Screenshot API documentation is found here: [https://docs.apiverve.com/api/webscreenshots](https://docs.apiverve.com/api/webscreenshots).  
You can find parameters, example responses, and status codes documented here.

### Setup

```
# Import the client module
from apiverve_websitescreenshot.apiClient import WebscreenshotsAPIClient

# Initialize the client with your APIVerve API key
api = WebscreenshotsAPIClient("[YOUR_API_KEY]")
```

---


### Perform Request
Using the API client, you can perform requests to the API.

###### Define Query

```
query = {  "url": "https://www.myspace.com/",  "type": "png",  "width": 1024,  "height": 600,  "fullpage": false }
```

###### Simple Request

```
# Make a request to the API
result = api.execute(query)

# Print the result
print(result)
```

###### Example Response

```
{
  "status": "ok",
  "error": null,
  "data": {
    "width": 1024,
    "height": 600,
    "scaleFactor": 1,
    "imageName": "b073a23b-3d80-4641-a6e0-440630915b05.png",
    "expires": 1722740935243,
    "url": "https://www.myspace.com/",
    "downloadURL": "https://storage.googleapis.com/apiverve.appspot.com/webscreenshots/b073a23b-3d80-4641-a6e0-440630915b05.png?GoogleAccessId=635500398038-compute%40developer.gserviceaccount.com&Expires=1722740935&Signature=ZSlwXOdQyER71uVEKATC0jw8aMdKqgdYa0qTQvKyjdhjHM5CyiNLzqzsq1aDp8y%2F9u9tOl%2Btuzgxm%2F7ho8YXMKRBvL0oMQjRhK%2FpwmBVI98ecMu2Z50hgtbEfLpUMAHN0Ld6D%2FKGSl7gPHS0lMSKhGHVJ1ory6HJ%2BKgpN2NcbfTuwNtLh1rbrLzrGW6WuRgqjrgrt2DCzuU5KPQPJmC4VvbZX98llTmjECdJmHZ2moh26AmzUJN3s4Z4eizm8zWpb%2BTTPHVPivPEmBfTQYb0N9kpVCDFAzTAKdI53weUkH4NGoe86Tdr7%2Bm1XqKw3t9Pi2IDhtU7iMFQ42cKmlEfBA%3D%3D"
  },
  "code": 200
}
```

---

## Customer Support

Need any assistance? [Get in touch with Customer Support](https://apiverve.com/contact).

---

## Updates
Stay up to date by following [@apiverveHQ](https://twitter.com/apiverveHQ) on Twitter.

---

## Legal

All usage of the APIVerve website, API, and services is subject to the [APIVerve Terms of Service](https://apiverve.com/terms) and all legal documents and agreements.

---

## License
Licensed under the The MIT License (MIT)

Copyright (&copy;) 2024 APIVerve, and Evlar LLC

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.