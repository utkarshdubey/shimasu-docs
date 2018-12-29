---
description: >-
  The Get Transcript API Route gets the transcripts of a youtube video passed in
  as an argument inside the link.
---

# Get Transcript API Route

{% api-method method="get" host="/api" path="/get\_transcript/:youtube\_video\_id" %}
{% api-method-summary %}
Get Transcript
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get free cakes.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="id" type="string" required=true %}
ID of the Youtube video to get.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Transcript successfully extracted. :\)
{% endapi-method-response-example-description %}

```javascript
[
    {
        "text": "[Music]",
        "start": 0.89,
        "duration": 3.15
    },
    {
        "text": "hi my name is John I lead the search and",
        "start": 5.24,
        "duration": 7.029
    },
    {
        "text": "she learning teams at Google well I",
        "start": 8.46,
        "duration": 5.969
    },
    {
        "text": "think it's amazingly inspiring that",
        "start": 12.269,
        "duration": 3.631
    },
    {
        "text": "people all over the world",
        "start": 14.429,
        "duration": 3.841
    },
    {
        "text": "I turned to search engines to ask",
        "start": 15.9,
        "duration": 3.9
    },
    {
        "text": "trivial questions and incredibly",
        "start": 18.27,
        "duration": 3.21
    },
    ...
]
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Third times a charm?
{% endapi-method-response-example-description %}

```text
This probably means that there are no captions available for the video, or, 
the video is not available.
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



