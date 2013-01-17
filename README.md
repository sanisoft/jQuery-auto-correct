jQuery-auto-correct
===================

The plugin to auto-correct words in textboxes or textareas as per given configuration like 'teh' to 'the', 'taht' to 'that', 'ur' to 'you are' etc.

Works with jQuery-1.7.2 on all latest versions of major browsers like Firefox, Seamonkey, Chrome, IE, Safari, Opera etc.

Configuration
-------------

Include plugin file (generally in 'head' tag), something like &lt;script src="jquery.autocorrect.js" type="text/javascript"&gt;&lt;/script&gt;

Configure your textboxes/textareas something like

```javascript
$(document).ready(function()
{
    $("#textbox1").autocorrect();

    $("#textbox2").autocorrect({
        corrections: {
            arent: "aren't",
            aboutit: "about it"
        }
    });

    $("#textarea").autocorrect({ corrections: { aboutit: "about it" } });
});
```

As you see, first textbox has auto-correct attached with no options, second with 'arent' (which already exists in default options but you can over-write it) and 'aboutit' (this is new one which does not exist in default corrections) then third one is textarea

Examples
--------

Please see examples.html
