<H1>Challenge 27: Client side validation is so secure?</h1>
<p>The main task of this challenge is to find the hidden password inside the
JavaScript.<p>
Steps:

1. View the source

2. Look for this block of code:
  ```javascript

			$(".c_submit").click(function(event) {
				event.preventDefault()
				var u = $("#cuser").val();
				var p = $("#cpass").val();
				if(u == "admin" && p == String.fromCharCode(74,97,118,97,83,99,114,105,112,116,73,115,83,101,99,117,114,101)) {
				    if(document.location.href.indexOf("?p=") == -1) {
				        document.location = document.location.href + "?p=" + p;
				    }
				} else {
				    $("#cresponse").html("<div class='alert alert-danger'>Wrong password sorry.</div>");
				}
			});
```
3. This line is important:
```javascript
if(u == "admin" && p == String.fromCharCode(74,97,118,97,83,99,114,105,112,116,73,115,83,101,99,117,114,101))
```
4. This line tell us that the password is the ascii code of the numbers. By using
an ascii chart we find that the password is **JavaScriptIsSecure**

5. Input the password in the password field and the flag will appear.
