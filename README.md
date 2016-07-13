Blogger Pager Script version 2.0

------ Guide --------------

- In Blogger > Go to Template > Edit HTML:
"Ctrl+F" for a search bar to find the this code: <b:include name='nextprev'/>

Now replace above code with below code:

<!-- Start Blogger Pager Script version 2.0-->
<!---<b:include name='nextprev'/>-->
<b:if cond='data:blog.pageType == &quot;index&quot;'>
<style type='text/css'>
.blogpager {font-size:1em; color:#49BA86; font-weight:bold; padding:0px 4px;}
.blogpager:hover{color:#398BC6;}
.TuePager input[type="text"]{ width: 10%; border: 1px solid #6FC89F; }
</style>
<div class"TuePager" align='center' style='margin:5px;'>
<form action='#' name='pager20'>
<span id='vwg-pager-first'/> <span id='vwg-pager-prev'/> <input name='showingpage' onfocus='this.select()' size='4' title='Enter page number that You want to go' type='text' value='init...'/>/<input disabled='disabled' name='pagestotal' size='4' type='text' value='init...'/> <input onclick='checkpager()' type='button' value='Go'/> <span id='vwg-pager-next'/> <span id='vwg-pager-last'/>
</form>
</div>
<script type='text/javascript'>
var blogID = &quot;YOUR-Blogger-blog-ID&quot;;
var home_page = &quot;http://YOURBlogNAME.blogspot.com/&quot;;
var pager_max_main = 7;
var pager_first_text = &quot;First&quot;;
var pager_last_text = &quot;Last&quot;;
var pager_prev_text = &quot;Prev&quot;;
var pager_next_text = &quot;Next&quot;;
</script>
<script src='URL of blogger_pager_script_v20.js' type='text/javascript'/>
</b:if>
<!-- END Blogger Pager Script version 2.0-->

*Note: 
- YOUR-Blogger-blog-ID: In your Blogger dashboard and take a look at your URL in browser address bar. You will now see a 19 digit unique identification number for your blog like this: ?blogID=5339405615560764967
- YOURBlogNAME: Your Blogspot Name.
Replace "URL of blogger_pager_script_v20.js" with your URL.
