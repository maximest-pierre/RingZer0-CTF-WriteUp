<H1> Challenge 30: Hashing is more secure? </H1>
<p>The main task for this challenge is to find the password hidden inside the javascript. As the name mentions, we are going to find the password inside of a hash.</p>
1. First step is to view the source.

2. Is to find the authentication script

3. Here is the script:
```javascript
$(".c_submit").click(function(event) {
				event.preventDefault();
				var p = $("#cpass").val();
				if(Sha1.hash(p) == "b89356ff6151527e89c4f3e3d30c8e6586c63962") {
				    if(document.location.href.indexOf("?p=") == -1) {   
				        document.location = document.location.href + "?p=" + p;
				    }
				} else {
				    $("#cresponse").html("<div class='alert alert-danger'>Wrong password sorry.</div>");
				}
			});
      ```
4. As you can see in the if statement it is true when the password is equal to the hash.
5. The hash is Sha1, there is a lot of web Decrypter for this type of hash.
6. The decrypted hash is: **adminz** (So original)
