# Lab

<script> document.cookie = "session=test GDPR"; document.cookie = "favorite_task=collect Data"; function alertCookie() { alert(document.cookie); } 

document.cookie = "name=oeschger; SameSite=None; Secure";
document.cookie = "favorite_food=tripe; SameSite=None; Secure";

function showCookies() {
  const output = document.getElementById('cookies')
  output.textContent = '> ' + document.cookie
}

function clearOutputCookies() {
  const output = document.getElementById('cookies')
  output.textContent = ''
}

</script>
<body> Bine ai venit la lab <button onclick="alertCookie()">Show cookies</button> 
<button onclick="showCookies()">Show cookies</button>

<button onclick="clearOutputCookies()">
  Clear
</button>

<div>
  <code id="cookies"></code>
</div>

</body>
