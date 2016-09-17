# jQuery Progressbarify
jQuery plugin to turn table cells into progress bars.

## Example Usage
```
$(document).ready(function(e){
    $('[data-progressbarify]').progressbarify();
});
```

Note: Progressbarify requires jQuery.


## Arguments
```
$.fn.progressbarify({
    targetColumn:    0,            // The column which the progress bar is applied to (default 0).
    primaryColour:   '#31b0d5',    // The colour of the left side of the bar (default #31b0d5).
    secondaryColour: 'transparent' // The colour of the right side of the bar (default transparent).
});
```
Note: The value of targetColumn can be given as the value of the `data-progressbarify` attribute on the table.

Note: To apply the progress bar to multiple columns you can chain progressbarify calls, like `$('#mytable').progressbarify({ targetColumn: 0 }).progressbarify({ targetColumn: 2 })`.

Note: The value of targetColumn should start at 0.
