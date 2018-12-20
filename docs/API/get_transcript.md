# Get Transcript API Route
The Get Transcript API Route gets the transcripts of a youtube video passed in as an argument inside the link.
```
/api/get_transcript/<youtube_video_id>
```
Replace the ``<youtube_video_id>`` with the ID of an actual Youtube Video.

## Example 1
Here is an example of a Youtube Video.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=LVV_93mBfSU
" target="_blank"><img src="http://img.youtube.com/vi/LVV_93mBfSU/0.jpg" 
alt="How internet works" width="240" height="180" border="10" /></a>

Its url is ``https://www.youtube.com/watch?v=LVV_93mBfSU`` where the id is ``LVV_93mBfSU``. After putting it in the url ``/api/get_transcript/<youtube_video_id>/`` we get the following result in json.

```json
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