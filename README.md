# Image Processing Project

Full Title:

<center>
<span style="font-size:large; font-weight:bold">
  Comparison of Image Enhancement Techniques applied to Sound Data Retrive( from Images )
</span>
</center>

Brief Description:

When an electromagnetic wave-type signal is capture or register, in his raw state, can be representated in multiple ways; but in the case it is a sound, despite the fact is a merly electrical field pertubation, can be also representated as an image; an image who contain the same informatin as the sound but in other information domains. (could have less informatio tho)

* * *

# Project Information

## Student Information

* **Name**: Jahir Gilberth Medina Lopez
* **USP Number**: 1659682

## Project Area(s)

### Main Area
  * Super-Resolution

### Secondariy Area(S)
  * Feature Extraction
  * In-painting
  * Noise Reduction [\*]
  * Image Restauration
  * Sound Processing [\*]

[\*] As an auxiliary topic.

## Project Context

### Project Idea

The main idea of the project is retrive damage images of sound data and return enchance sound data, the images are generated from sound signals.
The sound signals it self can be converted to images, but, during the sound data reception its possible to get analog images (as frecuency "pictures" of sound, like an analog tv). This redundant data could help in the enhacement sound procces, not only improving the sound qualty filtering the sound data, also filtering the image data asociated to the soud 

### Data Sources

#### University of Twente

[Wide-band WebSDR - Web Page](http://websdr.ewi.utwente.nl:8901)

The University of Twente posses a short-wave receiver located at the amateur radio club ETGD offices, who is offered free as an online radio.

![]( ./md-media/site-capture.png "Site Capture")

They allow the possibility of multiple tune-it radio frequency, generating a wide spectrum of available frequencies [0 Mhz - ~30 Mhz]


![]( ./md-media/general-data.png "24 Hours Frequencies Register")

Like it is looks, the image resulting of a complete day of registering frequencies posses a relative "pattern" behavior, in spite of it contents a lot of voice signals [ 0Mhz - 15 Mhz ].

#### The ARSS Project

[The ARSS Project - Web Page](http://arss.sourceforge.net)

The ARSS Project could be considerer as the main inspiration for this project, it works the idea of sound reconstruccion from images, however, the project was first develop for Sound-to-Image conversion.

The way it is works is converting images as if it were a frecuency domain data, this method of Sound-from-Image Data Retrive method is generic enough to convert any image to sound, being usefull in this project.

[The ARSS Project - Examples](http://arss.sourceforge.net/examples.shtml)

<center>
  <img src="http://arss.sourceforge.net/examples/lena/lena_small.png" alt="Lena" style="width:120px;height:120px;">
  <img src="./md-media/bidirectional.png" style="width:40px;height:40px;">
  <audio controls="controls">
    <source type="audio/mp3" src="http://arss.sourceforge.net/examples/lena/lena.mp3"></source>
    <p>Your browser does not support this audio format (MP3).</p>
  </audio>
</center>


## Project Objective(s)

### Pricipal Objective

<center>
<span style="font-size:large; font-weight:bold">
  Find what method statisticalid perfom better in the process of image enhance.
</span>
</center>
  

**The Project perfoms 3 diferent test :**

1. Using data to test every method chosed , getting the best and the worst methods (quality of results)
2. Using the methods obtained, aplying the same methods and comparing the accuracy of the "quality prediction"
3. Testing the methods in data who were not used in any of the steps before

**Types of Data**
  
  1. General Image:
    This kind of image represents the original data (sound) with compression in the time domain; representing, for example, 1 hour in an *2min length* image.
    ![]( ./md-media/general-data.png "General Image - 24 Hours")
  2. Detailed Image:
    This kind of image represents the original data (sound) without compression in the time domain
    ![]( ./md-media/detailed-data.png "Detailed Data 1 - Same bitrate")
    ![]( ./md-media/sound-plt.png "Detailed Data 2 - Same bitrate")
  3. Specific Data:
    Is just the sound data, it is considered as an original becaus his purpose is being the quality references in any of the tests.

<center>
  [Specific Data (Sound File Sample)](./md-media/audio_player.html)
  <audio controls="controls">
    <source type="audio/mp3" src="./md-media/websdr_recording_start_2018-05-17T00_10_41Z_7076.8kHz.mp3"></source>
    <source type="audio/ogg" src="./md-media/websdr_recording_start_2018-05-17T00_10_41Z_7076.8kHz.ogg"></source>
    <p>Your browser does not support this audio format (MP3 / OGG).</p>
  </audio>
</center>

### Secondary Objectives
  * Also test the effiency in developing time and excution time

  * Compare the "human percibed" quality, because , having an 99% of accuracy not always mean have a nice sound

## Solution Steps
  * Get all the possible "General Data" that it gonna be use [Picture Above] ( 50~100 samples)

    2016-02-01  : http://websdr.ewi.utwente.nl:8901/fullday/day16832.png

    *Using some music samples for the "human" quality test*

  * Get the sub samples relatives to the indefied patterns in the general data
  * Find Match between all of them (same pattern) an proceed to increase de number of samples
  * Start the tests
  * Compare
  * Get Results

The especific methods that are gonna be used , for now , are just tentative, for avoid innecesary changes in this section. they are just gona be adding when they are developed (all of them with his respective background)

# Project Development

# Project Results