---
title: Animations
index: 4
---

<ul class = "demos animations">
    <span>Included animations:</span>
    <li title = "I am the default" class = "animation columns medium-3"><span><strong>Bounce</strong></span></li>
    <li data-options="animation:fade" title="Cool ay" class = "animation columns medium-3"><span><strong>Fade</strong></span><i class="countdown"></i></li>
    <li title = "Whoop" data-options="animation:material" class = "animation columns medium-3"><span><strong>Material</strong></span></li>
    <li title = "Noice" data-options="animation:float" class = "animation columns medium-3"><span><strong>Float</strong></span></li>
</ul>
<ul class = "subsection">
    <h4>4.1 Defining custom animations</h4>
     <p>As I intended this to be a lightweight plugin, there isnt a gazillion choices of animations. But you can create one quite easily! <br /><small class="note">Material and the Float are actually custom animations in design, but I thought they looked pretty cool, so I included them in the plugin anyways <img src="{{ "assets/demo/img/trollface.jpg" | relative_url }}" /></small></p>
    <ul class="steps">
       <li>
           <span class="instruction">1. Specify the name of your custom animation</span><pre class="js">
           <code>var tooltip = new Drooltip({
   ...
   "animation": "myCustomAnimation",
   ...
});</code> 
          </pre>
       </li>
       <li>

           <span class="instruction">
           2. Create the relevant function; There will be 3 parameters that'll be passed to your function: 
           <ul class = "param_specification">
                <li><span>fn</span>Str <i>"animate"</i> |  <i>"deanimate"</i></li>
                <li><span>data</span>Object {<i class="params" title="Unique tooltip id">id</i>, <i class="params" title="Target DOM element">source</i>, <i class="params" title="Tooltip DOM element">tooltip</i>, <i class="params" title="Options associated with tooltip">options</i>}</li>
                <li><span>callback</span></li>
                <div class = "context">
                  <span>Context:</span>
                  <li><span>this</span>Object <i class="params" title="The object created from the initialisation; This gives you access to its public function">instance</i></li>
                </div>
           </ul>
           </span>
          <pre class="js">
          <code>function myCustomAnimation(fn, data, callback){
    var obj = this; // context => Drooltip Instance
    // There should be 2 paths basically
    if ( fn === "animate" ) {
    obj.hideAllTooltips();
    setTimeout(function(){
    data["tooltip"].classList.add("myCustomCSSAnimation")
    ... do some other cool stuff here ...
    if ( callback !== null || window[callback] !== undefined ) {
        window[callback](); // call the callback function
    }
    }, 200)
    } else if ( fn === "deanimate" ) {
    ... perform the deanimation here ...
    }
}</code> </pre>
       </li>
    </ul>
</ul>