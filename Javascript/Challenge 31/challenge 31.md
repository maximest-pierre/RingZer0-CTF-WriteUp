<H1> Challenge 31: The obfuscation is more secure </H1>
<p>The main task is to find the password hidden inside the script.</p>
1. First step is to view the source.

2. Is to find the authentication script

3. The script looks like a bunch of random value.

4. The technic use to hide the data is call obfuscation.

5. We need to convert the script into something more readable for humans. I used this site to make more readable. http://jsbeautifier.org/

6. Here is the script:
``` javascript
var _0xc360 = ["\x76\x61\x6C", "\x23\x63\x70\x61\x73\x73", "\x61\x6C\x6B\x33", "\x30\x32\x6C\x31", "\x3F\x70\x3D", "\x69\x6E\x64\x65\x78\x4F\x66", "\x68\x72\x65\x66", "\x6C\x6F\x63\x61\x74\x69\x6F\x6E", "\x3C\x64\x69\x76\x20\x63\x6C\x61\x73\x73\x3D\x27\x65\x72\x72\x6F\x72\x27\x3E\x57\x72\x6F\x6E\x67\x20\x70\x61\x73\x73\x77\x6F\x72\x64\x20\x73\x6F\x72\x72\x79\x2E\x3C\x2F\x64\x69\x76\x3E", "\x68\x74\x6D\x6C", "\x23\x63\x72\x65\x73\x70\x6F\x6E\x73\x65", "\x63\x6C\x69\x63\x6B", "\x2E\x63\x5F\x73\x75\x62\x6D\x69\x74"];
$(_0xc360[12])[_0xc360[11]](function() {
    var _0xf382x1 = $(_0xc360[1])[_0xc360[0]]();
    var _0xf382x2 = _0xc360[2];
    if (_0xf382x1 == _0xc360[3] + _0xf382x2) {
        if (document[_0xc360[7]][_0xc360[6]][_0xc360[5]](_0xc360[4]) == -1) {
            document[_0xc360[7]] = document[_0xc360[7]][_0xc360[6]] + _0xc360[4] + _0xf382x1;
        };
    } else {
        $(_0xc360[10])[_0xc360[9]](_0xc360[8]);
    };
});
```
7. As we can see the variable "_0xc360" is an array that contains Hexadecimal value.

8. The if condition ```if (_0xf382x1 == _0xc360[3] + _0xf382x2)``` is true when the value of the password is the third index of "_0xc360" and the content of _0xf382x2 which is the second index of "_0xc360".

9. With the hexadecimal value we convert it into ASCII symbol and there is the password. ***0211alk3***
