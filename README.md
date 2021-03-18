# YouTube-Captions-Subtitles-Extracter

This is a small Bookmarklet that extracts captions from a Youtube Video (if exists) and opens a panel on the right side of the page to display all the captions.

## Bookmarklet

[Bookmarklet-wiki](https://en.wikipedia.org/wiki/Bookmarklet):
A bookmarklet is a bookmark stored in a web browser that contains JavaScript commands that add new features to the browser. Bookmarklets are unobtrusive JavaScripts stored as the URL of a bookmark in a web browser or as a hyperlink on a web page. Bookmarklets are usually JavaScript programs. Regardless of whether bookmarklet utilities are stored as bookmarks or hyperlinks, they add one-click functions to a browser or web page. When clicked, a bookmarklet performs one of a wide variety of operations, such as running a search query or extracting data from a table. For example, clicking on a bookmarklet after selecting text on a webpage could run an Internet search on the selected text and display a search engine results page.

Example usage :
<a href="javascript:(function() {
function se(d) {
    return d.selection ? d.selection.createRange().text : d.getSelection()
} 
s = se(document); 
for (i=0; i<frames.length && (s==null || s==''); i++) s = se(frames[i].document); 
if (!s || s=='') s = prompt('Enter%20search%20terms%20for%20Wikipedia',''); 
open('https://en.wikipedia.org' + (s ? '/w/index.php?title=Special:Search&search=' + encodeURIComponent(s) : '')).focus();
})();">Wiki Search Page</a> (Drag to bookmark bar)

-

- like subtitles
- arrange them in groups and keep them on the screen until the next one is available.
- maybe anomaly detection | tree cluster based on closeness of the time stamp
- use pauses between words to differentiate the sentences.

- use them as [Bookmarklet-wiki](https://en.wikipedia.org/wiki/Bookmarklet)

- this can be used in youtube video as subtitles
- @feature: organize into centances by using std or tree clustering method to combine each word into readable subtitle
- @feature: divide web page into 2 and on the left open the subtitle
- @feature: divide web page into 3: one left yuotube and 2 inthe right. upper is the text and in the buttom is the translation of the subtitle.
- @feature: signature to "@author" find a text handwriting and link to repository

- Check auto google translate code of this [website](https://bestsale.be/index.php?route=product/manufacturer)
