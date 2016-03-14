VideoSubtitles
==================
2016-03-13


Tools to work with subtitles.



VideoSubtitles can be installed as a [planet](https://github.com/lingtalfi/Observer/blob/master/article/article.planetReference.eng.md).





- Srt to array: converts an srt file to an array with the following entries (example values in parenthesis):

        - id: a number representing the id of the subtitle (2)
        - start: float, the start time in seconds (24.443)
        - end: float, the end time in seconds (27.647)
        - startString: the start time in human readable format (00:00:24.443)
        - endString: the end time in human readable format (00:00:24.647)
        - duration: the duration of the subtitle, in ms (3204)
        - text: the text of the subtitle (<i>the Peacocks ruled over Gongmen City.</i>)
        

Example
-----------

```php
<?php

use VideoSubtitles\Srt\SrtToArrayTool;


require_once "bigbang.php"; // start the local universe
    

$f = "/path/to/kungfupanda2.srt";
$ret = SrtToArrayTool::getArrayByFile($f);
az($ret);
    
```



History Log
------------------
    
- 1.0.0 -- 2016-03-13

    - initial commit
    

    



