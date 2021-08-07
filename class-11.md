# CSS images 

we can make images as a background in our elemets and add properties for it 

```
ElementSselector{
    background-imag : url (img directory or link);

    background-repeat : repeat-x ; //to repeat horizantally
    background-repeat : repeat-y ; //to repeat vertically
    background-repeat : repeat ; // both 
    background-repeat : no-repeat ; 

    background-attachment : fixed ; // img stay at the same position
    background-attachment : scroll; // scroll with the user

    background-position : left top
                          left center
                          left bottom
                          right top
                          right center
                          right bottom
                          center top
                          center center
                          center bottom;
}
```


# Practical Information

- google analytics : tool used to know more about your website visitors
- to lanch your wbsite you should buy a domain name and a server(host)
- domain name is the name of your website in the web (annual fee)
- servier : is a large computer hosting your web page and make it accessible online (monthly fee)

# audio and vedio in HTML 

we can add audio to html by write `video` tag includes `source` tags 

```
<video controls>
  <source src="rabbit320.mp4" type="video/mp4"> // this for the video
  <source src="rabbit320.webm" type="video/webm"> // tis for the audio 
</video>
```

this example was from [MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs#html5_video_and_audio)

for a video we can add buttons using html add style to the buttons using css and then add functionality related to the video play , pause , stop and more proprties using CSS 