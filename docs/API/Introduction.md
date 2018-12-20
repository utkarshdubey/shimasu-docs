# Introduction
The API is built on top of Django framework(*v2.1*) for Python 3. The API currently doesn't support token authentication but it is clear that it would do in very soon. Until token authentication is implemented the API is free to use and experiment with. The various API endpoints are listed below. Notice it would require the ID of the youtube video instead of the full url. The ID can be derived from the url itself. Just copy the part after ``youtube.com/watch?v=...`` before any ampersands(&).

```
/api/get_transcript/<youtube_video_id>
/api/get_suggestions/<youtube_video_id>
```

The API returns data in JSON format. You can use [Postman](https://getpostman.com) to tinker with the API. For more information about using Postman please read their documentation or this simple [Tutorial](https://developer.mypurecloud.com/api/rest/postman/).
