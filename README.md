# readyfor.js
jQuery on ready helper plugins.

## Simple Usage Rails Example

Add id/class to your body tag as follows:

<pre>
  &lt;body id="&lt;%= controller_name -%&gt;-controller" class="&lt;%= action_name -%&gt;-action"&gt;
</pre>

## Trigger on ready events..

### Explicitly

<pre>
  $(document).ready_for_selector("#awesome-controller.show-action", function() {
    "use strict";
    .
    .
    .
  });
</pre>

### With some helpers....

<pre>
  $(document).ready_for_controller("awesome", function() {
    "use strict";
    .
    .
    .
  });
  
  $(document).ready_for_controller_action("awesome", "show", function() {
    "use strict";
    .
    .
    .
  });
</pre>