---
title: Useful functions
index: 8
---

The following are some functions you may find useful especially when creating custom animations/triggers


<table>
<thead>
    <tr>
        <th style="width:300px;">Function</th>
        <th>Description</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>animateAllTooltips()</td>
        <td>
            Animate all tooltips associated in the instance
        </td>
    </tr>
    <tr>
        <td>deanimateAllTooltips()</td>
        <td>
           Deanimate all tooltips associated in the instance
        </td>
    </tr>
    <tr>
        <td>animateTooltip(<span class="fnParams" title="The data object that was passed to your function">data</span>)</td>
        <td>
            Animate an individual tooltip
        </td>
    </tr>
    <tr>
        <td>deanimateTooltip(<span class="fnParams" title="The data object that was passed to your function">data</span>)</td>
        <td>
            Deanimate an individual tooltip
        </td>
    </tr>
    <tr>
        <td>showAllTooltips()</td>
        <td>
           Show all tooltips of that instance (no animation)
        </td>
    </tr>
    <tr>
        <td>hideAllTooltips()</td>
        <td>
           Hide all tooltips of that instance (no animation)
        </td>
    </tr>

    <tr>
        <td>showTooltip(<span class="fnParams" title='Tooltip DOM, data["tooltip"]'>tooltip</span>)</td>
        <td>
           Show a specific tooltip
        </td>
    </tr>
    <tr>
        <td>hideTooltip(<span class="fnParams" title='Tooltip DOM, data["tooltip"]'>tooltip</span>)</td>
        <td>
           Hide a specific tooltip
        </td>
    </tr>
    <tr>
        <td>addStandardEffect(<span class="fnParams" title='Tooltip DOM, data["tooltip"]'>tooltip</span>, <span class="fnParams" title='The included effect that you want to add'>effect</span>)</td>
        <td>
          	Animate the tooltip with an <span class="underline defaultTooltip" title="Bounce, Fade, Material, Floating">included effect</span>
        </td>
    </tr>
    <tr>
        <td>removeStandardEffect(<span class="fnParams" title='Tooltip DOM, data["tooltip"]'>tooltip</span>, <span class="fnParams" title='The included effect that you want to remove'>effect</span>)</td>
        <td>
          	Denimate the tooltip with an <span class="underline defaultTooltip" title="Bounce, Fade, Material, Floating">included effect</span>
        </td>
    </tr>
    <tr>
        <td>showArrow(<span class="fnParams" title='Tooltip DOM, data["tooltip"]'>tooltip</span>)</td>
        <td>
          	Show the tip arrow of a tooltip
        </td>
    </tr>
    <tr>
        <td>hideArrow(<span class="fnParams" title='Tooltip DOM, data["tooltip"]'>tooltip</span>)</td>
        <td>
          	Hide the tip arrow of a tooltip
        </td>
    </tr>
    <tr>
        <td>updatePosition(<span class="fnParams" title='The data object passed to your function'>data</span>)</td>
        <td>
          	Intelligently update the position of a tooltip relative to its target element
        </td>
    </tr>
</tbody>
</table>



<ul style="margin-top:30px" class="steps">
    	<li>
    		<span class = "instruction">An example on how to use the function</span>
    		<pre class = "js"><code>var tooltip = new Drooltip({ ... })
tooltip.animateAllTooltips();
</code></pre>    
		</li>
	</ul>