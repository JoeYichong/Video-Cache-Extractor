# Video Cache Extractor

**Video Cache Extractor** is an application that extracts cached MPEG-TS fragments from the Chrome cache directory
and reconstructs a single video file.

### Quickstart 
You can use the following command to extract an online video from the Chrome cache directory:
```
>>> extract -t fileTag -a 15:00:00 -co
```
* ``-t fileTag`` adds tag `fileTag` to the file name of the final video file. 
* ``-a 15:00:00`` the video fragments cached/created after the time `15:00:00` will be collected.
* ``-co`` means that all the video fragments collected will be deleted after merged into a single file.
* Press **``Enter``** to stop collecting video fragments.

### Configuration
`config.properties` is the configuration file.
* `dir.cached` - Your local Chrome cache directory.
* `dir.collected` - The directory where the collected fragments are stored.
* `dir.generated` - The directory that keeps the generated video files.


