I can no longer edit a certain note in my gospel library notes on the web.

I have noticed this error happens at different times, and the response body is as follows: 

```
<html><body><center><h1><b>Not Available</b></h1><i>This page is unavailable.  Error code: 2-1919</i></center></body></html>
```

Other times that this error often occurs (or something like it) is when I copy and paste a url that has the improper &lang=eng rather than the ?lang=eng as a query parameter in the url. For some reason, urls like that in the gospel library note causes it to break the json.

The request (in the form of a fetch) is shown below. I have hard refreshed my browser: google chrome, which is up to date with the latest version. 


```javascript
fetch("https://www.churchofjesuschrist.org/notes/api/v3/annotations/c54acdd2-7f28-4314-8b81-dcd384d5496d/note", {
  "headers": {
    "accept": "application/json",
    "accept-language": "en-US,en;q=0.9",
    "content-type": "application/json",
    "sec-ch-ua": "\"Chromium\";v=\"110\", \"Not A(Brand\";v=\"24\", \"Google Chrome\";v=\"110\"",
    "sec-ch-ua-mobile": "?0",
    "sec-ch-ua-platform": "\"Windows\"",
    "sec-fetch-dest": "empty",
    "sec-fetch-mode": "cors",
    "sec-fetch-site": "same-origin"
  },
  "referrer": "https://www.churchofjesuschrist.org/notes",
  "referrerPolicy": "strict-origin-when-cross-origin",
  "body": "{\"content\":\"<div>Study on light [noun]</div><div><br></div><div>I personally want to study this because of the interesting interaction between light, good, faith, growth, enlightenment, truth, and the word; as discussed in Alma 32. </div><div><br></div><div>Similar TG groups are everywhere.</div><div><br></div><div>Light:</div><ul><li>Is good </li><li>Is sweet</li><li>Is pleasant to behold (especially physical light)</li><li>God created it and the sources of it </li><li>Is a physical light often, or light source (like the sun/moon)</li><li>Is a necessity to do anything (you can't move pretty much without light)</li><li>Christ is likened to the light of the morning</li><li>Christ is our light</li><li>\\\"For with thee <i>is</i> the fountain of life: in thy light shall we see light.\\\" We discern light as we have more of Christ's light (the light of Christ?). </li><li>Brings forth righteousness</li><li>Light and truth: <a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/ps/43?id=3#p3\\\">seems that both lead us</a>. So each has a role to play, and they are different things. </li><li><a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/ps/118?id=27#p27\\\">God shows us </a>light. </li><li>The <a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/ps/119?id=105#p105\\\">word of God is a lamp to our feet, and a light to our pat</a>h in life. </li><li><a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/prov/4?id=18#p18\\\">Our path, if we are just, is like a shining light, which shines more until the perfect day</a>. </li><li>You can walk/live/act in the light of Christ. </li><li>Darkness is the contrary of light</li><li>It can be inside us. <a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/isa/50?lang=eng&id=10#p10\\\">We have light inside us as we trust Christ and God.</a> It seems this is our light, which is effected by our spirituality; <a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/isa/58?lang=eng&id=8#p8\\\">in this example our light breaks forth as the morning during/after a true fast</a>, and <a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/isa/60?lang=eng&id=1#p1\\\">here it seems (from prior verses and this verses) that the keeping of our latter-day covenants with Christ allow our light to shine</a>.</li><li><a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/bofm/2-ne/18?lang=eng&id=20#p20\\\">An absense of light in people is the cause of people not being willing to hearken to God's law or His word</a>. </li><li><a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/micah/7?id=p8-p9&lang=eng#p8\\\">We can be surrounded by darkness of sorts, yet feel light from God</a>, or he will be a light unto us. </li><li><a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/bofm/2-ne/15?lang=eng&id=20#p20\\\">We can make things that are dark/light seem opposite to ourselves or others; or deceive ourselves</a>. </li><li>If we walk in our own light, rather than God's light, <a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/isa/50?lang=eng&id=11#p11\\\">we'll end up unhappy</a>. </li><li>Physical light from the sun, moon, and starts will be diminished or completely gone during certain phases near the prophesied 2nd coming.</li><li><a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/isa/60?lang=eng&id=19#p19\\\">Christ will be Zion's light</a> when the sun and moon no more give physical light. </li><li>Our keeping of covenants allow us to be lights for others; eg. <a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/isa/42?lang=eng&id=6#p6\\\">isaiah</a>, <a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/isa/49?lang=eng&id=6#p6\\\">here as in missionary work</a> (<a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/nt/acts/13?lang=eng&id=47#p47\\\">and this too</a>, and <a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/isa/60?lang=eng&id=3#p3\\\">here</a>, ), and <a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/dc-testament/dc/86?lang=eng&id=11#p11\\\">includes being through the priesthood a savior to God's people Israel</a>,</li><li>God <a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/isa/45?lang=eng&id=7#p7\\\">forms</a> the light (don't know if that means he creates it from nothing? Because it seems like God divides the light from the darkness in the creation; as if He is the enabler of light to shine forth and have direction/aim.)</li><li>Daniel was full of it; <a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/dan/5?lang=eng&id=14#p14\\\">light is mentioned next to his understanding and excellent wisdom</a>. </li><li>Depending on our righteousness, it seems that <a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/amos/5?lang=eng&id=18#p18\\\">certain days of judgement or other events will be either \\\"light\\\" or \\\"darkness\\\" to us</a>. E.g. the second coming or judgement day.</li></ul><div><br></div><div>Hard to understand references of light: </div><ul><li>This references david being blessed with still having the tribe of Judah after his son Solomon would lose the empire. <a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/1-kgs/11?id=36#p36\\\">https://www.churchofjesuschrist.org/study/scriptures/ot/1-kgs/11?id=36#p36</a>.</li><li>A note from job, where the light is as darkness. Like the light is no longer light? <a href=\\\"https://www.churchofjesuschrist.org/study/scriptures/ot/job/10?id=22#p22\\\">https://www.churchofjesuschrist.org/study/scriptures/ot/job/10?id=22#p22</a> </li><li></li></ul>\"}",
  "method": "PATCH",
  "mode": "cors",
  "credentials": "include"
});
```

The errors in the javascript developer console say the following:

```
9UX54-L57TE-34QD8-DURP5-GFD2R:10 fetchHelper error SyntaxError: Unexpected token '<', "<html><bod"... is not valid JSON
BOOMR_plugins_errors_console_error @ 9UX54-L57TE-34QD8-DURP5-GFD2R:10
Bp @ fetchHelper.js:66
Promise.catch (async)
(anonymous) @ annotations.js:86
(anonymous) @ annotations.js:42
(anonymous) @ index.js:16
i @ App.js:100
(anonymous) @ Annotation.js:225
(anonymous) @ HtmlEditor.js:162
l @ index.js:27
setTimeout (async)
c @ index.js:38
(anonymous) @ RichTextEditor.js:95
ns @ react-dom.production.min.js:211
hl @ react-dom.production.min.js:257
t.unstable_runWithPriority @ scheduler.production.min.js:19
Ho @ react-dom.production.min.js:122
pl @ react-dom.production.min.js:257
(anonymous) @ react-dom.production.min.js:256
z @ scheduler.production.min.js:17
S.port1.onmessage @ scheduler.production.min.js:14
VM3147:1 Uncaught (in promise) SyntaxError: Unexpected token '<', "<html><bod"... is not valid JSON
```