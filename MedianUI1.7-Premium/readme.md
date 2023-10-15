To use modified theme.xml, do following steps:
1. ##### Open Blogger Layout -->
2. #### --> Widget: Header Notification -->
```
<script>
	window.onload = function() {
		localStorage.setItem("mode", "darkmode")
		if (localStorage.getItem("mode") === "darkmode"){
			document.querySelector("#mainContent").classList.add("darkMode")
		}else{
			document.querySelector("#mainContent").classList.remove("darkMode")
		}
		
		
		var blogTitleElement = document.getElementById("blogTitle");
		blogTitleElement.innerHTML += " " + document.title;
	};   
</script>


<!--[ Alternatif content with button link ]-->
<div class='notifAlt'>
  <span id="blogTitle">
    Welcome to
  </span> 
  <a href='https://www.youtube.com/@ONISTIDA?themeRefresh=1' target='_blank' rel='noopener'>Visit: Onistida YT</a>
</div>

<style>
.PopularPosts h3 {
  font-size: 14px; /* Adjust the value to your desired font size */
</style>
```
