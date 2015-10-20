# jQuery-mTab
This jQuery plugin provides responsive tab functionality. The tabs transform to an accordion when it reaches a CSS breakpoint
<ul>
  <li>Tabs transform to accordion based on breakpoint</li>
  <li>Uses CSS for tab switching animation (true/false)</li>
  <li>Uses CSS for the desktop/tablet/mobile view</li>
  <li>Has callback events for the tab events</li>
  <li>Accordion are collapsible</li>
  <li>Set custom active class</li>
  <li>Set default active/open tab</li>
  <li>Tabs can be opened with URL hashes</li>
  <li>Tabs can auto rotate</li>
  <li>Accordion will scroll to respective click scroll top position</li>
  <li>Tabs can be collapsed (optional)</li>
  <li>Tabs can start collapsed based on the view (optional)</li>
  <li>Cross browser compatibility (IE7+, Chrome, Firefox, Safari and Opera)</li>
  <li>Multiple device support (Web, Tablet, Mobile, etc)</li>
</ul>

<h2>How to Use</h2>
<ul>
  <li>Requires jQuery (minimaly jQuery 1.9.2)</li>
  <li>Include jquery-mTab-min.js</li>
</ul>
<p>
<pre>&lt;script src="js/jquery-mTab-min.js"&gt;&lt;/script&gt;</pre>
</p>
<p><strong>Include mTab-style.css for the basic Tabs to Accordion switching</strong></p>
<p>
<pre>&lt;link type="text/css" rel="stylesheet" href="css/mTab-style.css" /&gt;
</pre>
</p>
<p> <strong>Use this HTML markup:</strong></p>
<p>
<pre>
&lt;div class="sectionTabbing"&gt;
    &lt;ul class="tabNav"&gt;
        &lt;li&gt;&lt;a href="#tab1"&gt; .... &lt;/a&gt;&lt;/li&gt;
        &lt;li&gt;&lt;a href="#tab2"&gt; .... &lt;/a&gt;&lt;/li&gt;
        &lt;li&gt;&lt;a href="#tab3"&gt; .... &lt;/a&gt;&lt;/li&gt;
    &lt;/ul&gt;
        &lt;div class="tabContainer"&gt;
        &lt;div class="tabContent" id="tab1"&gt; ....... &lt;/div&gt;
        &lt;div class="tabContent" id="tab2"&gt; ....... &lt;/div&gt;
        &lt;div class="tabContent" id="tab3"&gt; ....... &lt;/div&gt;
    &lt;/div&gt;
&lt;/div&gt;
</pre>
</p>
<p> Use this jQuery function to enable responsive tabs on the selected element:</p>
<p>
<pre> // Default Setting
$('.sectionTabbing').mTab({
     navigation: ".tabNav"
    ,container: ".tabContainer",
    ,activeTab: 1
    ,activeClass: "active" 
    ,scrollOffset: true
    ,accordScreen: 768
    ,animation: 700
    ,toggleClose: false
    ,openWithUrl: false
    ,callbackonclick: function() {}
     callback: function() {} 
});
</pre>
</p>
