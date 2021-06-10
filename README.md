Elix scapper for french sign language for Anki cards.

Interactive notebooks for choosing each definition by hand, or batch notebooks to download all words of a list.

Here is an example of such Anki deck: https://ankiweb.net/shared/info/1368632736


Note that once you run the notebooks, the text content will be stored in a csv file. You need a Anki template to receive it, I recommend you use the one provided in my Anki deck (see link above).

The videos will be stored in another folder. You should optimize a bit the videos
You can use ffmpeg likewise:

```bash
ffmpeg -i input.mp4 -vcodec libx264 -crf 40 output.mp4
```

You can do a bash for loop to process all videos.

Then, once the csv is imported in Anki, you need to copy the video files into the media folder of your Anki. Warning! The videos names must have the name in the last column of the csv (format is `[sound:VIDEONAME]`).

If you scrap Elix, keep a time sleep between request, and try to do it outside peak hours (better to launch it during the night). You wouldn't want to break such a wonderful website.