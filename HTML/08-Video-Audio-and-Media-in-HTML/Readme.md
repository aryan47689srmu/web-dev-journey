# Video, Audio, and Media in HTML

## &#x20;Introduction

HTML provides built-in elements to embed multimedia content like **videos, audio files, and other media** directly into web pages without requiring external plugins. This makes modern websites more interactive and engaging.

---

# &#x20;Video in HTML

## &#x20;`<video>` Tag

The `<video>` tag is used to embed video files in a webpage.

### &#x20;Basic Syntax

```html
<video src="video.mp4" controls></video>
```

### &#x20;Example

```html
<video width="400" height="300" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>
```

### &#x20;Important Attributes

| Attribute      | Description                       |
| -------------- | --------------------------------- |
| controls       | Adds play, pause, volume controls |
| autoplay       | Plays video automatically         |
| loop           | Repeats the video                 |
| muted          | Mutes the video                   |
| width / height | Sets size of video                |

---

# &#x20;Audio in HTML

## &#x20;`<audio>` Tag

The `<audio>` tag is used to embed sound files.

### &#x20;Basic Syntax

```html
<audio src="audio.mp3" controls></audio>
```

### &#x20;Example

```html
<audio controls>
  <source src="sound.mp3" type="audio/mpeg">
  <source src="sound.ogg" type="audio/ogg">
  Your browser does not support the audio element.
</audio>
```

### &#x20;Important Attributes

| Attribute | Description             |
| --------- | ----------------------- |
| controls  | Displays audio controls |
| autoplay  | Plays automatically     |
| loop      | Repeats audio           |
| muted     | Starts muted            |

---

# &#x20;Media Elements in HTML

## &#x20;`<source>` Tag

* Used inside `<video>` and `<audio>`
* Specifies multiple file formats for compatibility

```html
<video controls>
  <source src="video.mp4" type="video/mp4">
  <source src="video.webm" type="video/webm">
</video>
```

---

## &#x20;`<track>` Tag

* Used for subtitles and captions in videos

```html
<video controls>
  <source src="movie.mp4" type="video/mp4">
  <track src="subtitles.vtt" kind="subtitles" srclang="en" label="English">
</video>
```

---

## &#x20;`<embed>` Tag

* Embeds external content like PDFs or multimedia

```html
<embed src="file.pdf" width="500" height="400">
```

---

## &#x20;`<iframe>` Tag

* Used to embed videos from other platforms (like YouTube)

```html
<iframe width="560" height="315"
src="https://www.youtube.com/embed/VIDEO_ID">
</iframe>
```

---

# &#x20;Supported Formats

## &#x20;Video Formats

* MP4 (Most widely supported)
* WebM
* OGG

## &#x20;Audio Formats

* MP3
* WAV
* OGG

---

# &#x20;Advantages of HTML Media

* No need for plugins like Flash
* Easy to use and integrate
* Works across modern browsers
* Supports controls and customization

---

# &#x20;Notes

* Always provide multiple formats for better browser compatibility
* Avoid using autoplay (can annoy users)
* Use subtitles for accessibility

---

# &#x20;Conclusion

HTML multimedia elements like `<video>` and `<audio>` make it simple to add rich media content to web pages. By using proper tags and attributes, developers can create engaging and user-friendly websites.

---
