# Lab
<script> document.cookie = "session=test GDPR"; 
  document.cookie = "favorite_task=collect Data"; 
  function alertCookie() { alert(document.cookie); } </script>
<body> Bine ai venit la lab <button onclick="alertCookie()">Show cookies</button> </body>
allCookies = document.cookie;
document.cookie = newCookie;
// Note that we are setting `SameSite=None;` in this example because the example
// needs to work cross-origin.
// It is more common not to set the `SameSite` attribute, which results in the default,
// and more secure, value of `SameSite=Lax;`
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
Copy to Clipboard
<button onclick="showCookies()">Show cookies</button>

<button onclick="clearOutputCookies()">
  Clear
</button>

<div>
  <code id="cookies"></code>
</div>
