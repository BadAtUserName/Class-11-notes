# Class-11-notes
I Video and audio on the web<br>

a. First influx of videos used flash or Silverlight both have security issues<br>
b. The < video > element<br>
     a.Similar to using an image tag<br>
c. Src same way as the image element<br.
d. Controls users must be able to control video and audio playback<br>
e. The paragraph inside the <video> tags is fallback content and will be displayed if browser if page doesn’t support video<br>
II. Using multiple source formats to improve compatibility<br>

A. Contents of a media file<br>
     a. Mp3, mp4, webM, called container formats<br>
                                                                           i.      Define the structure in which the audio or video tracks that make up media are stored along with metadata describing the media<br>
                                                                         ii.      webM file contain movie has main video track and one alt angle track plus audio for eng and span.<br>
                                                                       iii.      Each audio track is encoded  audio codec <br>
                                                                       iv.      Video encoded using a video codec<br>
Codecs exist to compress video and audio into manageable files<br>
                                                                           i.      Each web browser supports an assortment of codecs<br>
                                                                         ii.      Each codec has own advantages and drawbacks<br>
                                                                       iii.      Things to keep in mind  mobile browsers support additional formats not supported by their desktop equivalents<br>
c. Each source element also has a type also has a type attribute/is optional but advised to use<br>
III. Other Video features<br>

A. Width and height<br>
B. Autoplay<br>
     a. Has video start playing right away<br>
C.Loop<br>
D.Muted<br>
E. Poster<br>
     a. URL of an image that is displayed before video is played<br>
F. Preload<br>
     a.Used for buffering large files takes 3 values<br>
                                                         i.      “none” does not buffer files<br>
                                                                         ii.      “auto” buffers the media file<br>
                                                                       iii.      “metadata”buffers only the metadata for the file

IV. The audio element<br>

Works just like video element<br>
Audio doesn’t support width and height<br>
V. Displaying audio tracks<br>

Many people can’t or don’t want  to hear audio/vid content<br>
many people have auditory impairments<br>
others may be in noisy surroundings<br>
similarly enviros might be too quiet<br>
people who don’t speak the lang may need translation<br>
Using HTML video can use webTVV to file format and the track element<br>
webVTT format for writing test files containing multiple strings of text along with metadata such as the time in the video at which each text string should be displayed<br>
Common Cues<br>
                                                               i.      Subtitles<br>
                                                             ii.      Captions<br>
                                                           iii.      Timed descriptions<br>
                                            
                                              
I.Responsive images<br>
Useful for things that are on different sized displays like phone or tablet<br>
II.                   How to create responsive imaging.<br>
Looking at 2 problems res switching and art direction<br>
                                                               i.      Resolution switching: diff sizes<br>
Can use two attributes srcset and sized to provide several addition source images alone<br>
Not hard to format as long as diff part of attribute on each line each val contains a comma separated list<br>
Srcset defines the set of images we will allow the browser to choose between and what each image size is<br>
Sizes defines a set of media condition and indicates what image size would be best to choose when certain media conditions are true.
When these attributes are in place the browser will<br>
Look at screen size/pixe density/zoom level/screen orientation/network speed
Work out which media  condition in the sized list is the first one to be true<br>
Look at the slot size given to the media query<br>
Load img reffed in the srcset list has same size as the slot or if there isn’t one first img bigger than the chosen slot size<br>
                                                             ii.      Resolution switching same size diff res.
When css has px set sizes not needed browser works out res. Serves most appropriate img<br>
                                                           iii.      Art direction involves wanting to change the image displaye to suit diff image display size<br>
Using <picture> can fix this issue<br>
Wrap whole source/img elements in <picture> tag<br>

Video and audio content

Explain how the ability to use video and audio on the web has evolved since the early 2000s.
A first video where possible using plugins like flash and Silverlight but they can be problematic and are now obsolete now we use html and js api’s
Describe the use of the src and controls attributes in the <video> element.
Src the source contains the path to the video you want same as when using it in an image. Controls give you the ability to control the video like like start stop and volume
Why is it important to have fallback content inside the <video> element?
It is important in the same way an alt on an image is important it make it more accessible to people.
Write a very short story where <audio> and <video> are characters.
Here is a story about two best friends, Audio and Video most of the time they do everything together and are very similar. One of their few differences that they don’t mind very much is the size video can make themselves, they can be tall, long, short, small. Audio is always the same size invisible.  Although sometimes they get too much hype, they know that they are supporting characters to make peoples experiences better.
Guide to Grid

How does Grid layout differ from Flex?
The difference between css grid and fles, flex is designed for layout in one dimesion either row or column. Grid is 2d rows and columns at the same time.
Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.
Grid container is the parent of all the grid items.
Gride items is the child of the grid elements
Grid line are the lines like rows or columns that  make up the grid.
Responsive Images

Besides making a site visually appealing across different screen sizes, why should developers make images responsive?
Responsive images help us avoid the art direction problem and the resize problem, it also saves us some time on page load.
Define the following <img> attributes srcset and sizes. Write an example of how they are used.
The Src tag defines the set of images the browser is allowed to choose from, and what size the images. It gives us some different sizes to use  when we load the page. Sizes gives us some options of what size we are going to use with it’s maxs available. 
How is srcset more helpful for responsive images than CSS or JavaScript?
The way pageload works means you wouldn’t be able to to dynamically change an image once it has been placed during page load.

 
