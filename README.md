# summernote-emoji
Summernote emoji plugin

![Screen Shot](https://tamit.info/plugins/summernote-emoji/example/ScreenShot.png)

**Demo** https://tamit.info/plugins/summernote-emoji/example
# Installation & Usage:
In your ```<head>``` section, add the following stylesheet links. Adjust the lib/css path to match yours.
```
<link href="tam-emoji/css/emoji.css" rel="stylesheet">
```
The end of your ```<body>``` section, add the following JavaScript links. This library depends on jQuery, so jQuery must also be included, before these scripts are run. Once again, adjust the tam-emoji/js path to match yours.
```
  <script src="tam-emoji/js/config.js"></script>
  <script src="tam-emoji/js/tam-emoji.min.js"></script>
```
Before add ```emoji``` to summernote toolbar.

# Example
```
<textarea id="summernote"></textarea>
```
```
$('#summernote').summernote({
  toolbar: [
		toolbar: [
            ['insert', ['emoji']],
            ['tool', ['undo', 'redo', 'codeview']]
        ]
	]
});
```

# Configuring Options
```
# Emoji Button
document.emojiButton = 'fas fa-smile'; // default: fa fa-smile-o

#The Emoji selector to input Unicode characters instead of images
document.emojiType = 'unicode'; // default: image

#Relative path to emojis
document.emojiSource = 'tam-emoji/img';
```
