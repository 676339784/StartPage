startpage
====

![example screenshot (150721)](https://raw.githubusercontent.com/676339784/676339784.github.io/master/StartPage/startpage%201%20dark.png)
![example screenshot expanded (150721)](https://raw.githubusercontent.com/676339784/676339784.github.io/master/StartPage/startpage%202%20dark.png)


<br>

##### Usage
The easiest way to make changes is by editing _config.json_ and _index.html_.

<br>
###### JSON
| attribute         | if true                                          |
| ----------------- | ------------------------------------------------ |
| borders           | enables borders on top and bottom                |
| alwaysopen        | makes all squares open on load                   |
| mascot            | enables image in the bottom right hand corner    |
| allowVersionCheck | allows to check for the latest Version on github |

The version is only checked for if the help popup shows up.

The _images_ array is a list of all mascot images to be used. If you want to use only one image just create an array with one item.

<br>
###### HTML
To add/remove a square just add/remove a _div .sqr_ within _div #cell_.<br>
Keep the structure like this:
```
<div class="sqr">
    <span>HEADING</span>
    <div class="content">
        <a href="URL">LINK TITLE</a><br>
        <a href="URL">LINK TITLE</a><br>
        ...
        <a href="URL">LINK TITLE</a>
    </div>
</div>
```

<br>
###### search
```
-d      DuckDuckGo
-g      Google (default)
-h      Shows this list
-l      Genius
-w      Wikipedia
-y      YouTube
```
The following example will search for _github_ using _Wikipedia_:<br>
-w github<br>
If an invalid search option or none at all is specified, Google is used.

