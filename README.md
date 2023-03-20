# DCII
Doigt's Code of Information Interchange is Doigt's own personal standard for written text on old machines that don't have an official standard for text encoding or for use cases which require supporting more than one alphabet. I don't care about your opinion if your opinion is "this shouldn't exist".

## Advantages

* Lightweight: The character values can be stored in 8-bit values.
* International: It supports multiple writing systems.
* Compact: With the special Uppercase character, we can still have lower and upper case characters while supporting many alphabets and having the lowest possible size for a single character.
* Adaptable: ~30 characters reserved for private use, which should give enough breathing room for special use cases.

## Special Characters

### Null
The null character indicates the end of a string for programming purposes. It shouldn't be displayed. It is not mandatory to use it in text data.

### Next line
Moves the cursor to the next line at column 0 of the text container. It's the equivalent to a new line.

### Uppercase
The way the uppercase character works is that the character which follows shoud be displayed in its capital form. If there are two consecutive uppercase characters, then all characters which follow are to be displayed in their uppercase form until another uppercase character or a null character is encountered.

In the case of Japanese text, the uppercase character changes the character set from katakana to hiragana instead. Hiragana is the default character set because, historically, katakana-only games far outnumber the hiragana-only games[¹](https://legendsoflocalization.com/video-games-and-japans-three-main-writing-systems/#writing-everything-in-katakana). However, if feedback wants hiragana as the default set, I will change it according to the feedback.

In the case of georgian text, only Mkhedruli is officially covered by DCII. So the uppercase character has no effect on georgian letters.

### Unknown
The unknown character is for conversion purposes in a case when a character from another encoding doesn't exist in DCII.

### Cyrillic, Greek and Armenian alphabets
In order to save some space, letters which share an identical or similar appearance to latin letters do not have their own code with the exception of characters which are identical or similar for only one of their forms. Diacritics don't exist in DCII. Greek texts should use the semi-colon as a substitute for question marks. The word-final sigma variant doesn't exist in this standard.

## The Table
|Hex|Dec|Glyph    |
|---|---|---------|
|0  |0  |Null     |
|1  |1  |Next Line|
|2  |2  |Uppercase|
|3  |3  |Space    |
|4  |4  |!        |
|5  |5  |#        |
|6  |6  |"        |
|7  |7  |'        |
|8  |8  |( or [   |
|9  |9  |) or ]   |
|A  |10 |*        |
|B  |11 |+        |
|C  |12 |,        |
|D  |13 |-        |
|E  |14 |.        |
|F  |15 |/        |
|10 |16 |:        |
|11 |17 |;        |
|12 |18 |?        |
|13 |19 |0        |
|14 |20 |1        |
|15 |21 |2        |
|16 |22 |3        |
|17 |23 |4        |
|18 |24 |5        |
|19 |25 |6        |
|1A |26 |7        |
|1B |27 |8        |
|1C |28 |9        |
|1D |29 |a or A   |
|1E |30 |b or B   |
|1F |31 |c or C   |
|20 |32 |d or D   |
|21 |33 |e or E   |
|22 |34 |f or F   |
|23 |35 |g or G   |
|24 |36 |h or H   |
|25 |37 |i or I   |
|26 |38 |j or J   |
|27 |39 |k or K   |
|28 |40 |l or L   |
|29 |41 |m or M   |
|2A |42 |n or N   |
|2B |43 |o or O   |
|2C |44 |p or P   |
|2D |45 |q or Q   |
|2E |46 |r or R   |
|2F |47 |s or S   |
|30 |48 |t or T   |
|31 |49 |u or U   |
|32 |50 |v or V   |
|33 |51 |w or W   |
|34 |52 |x or X   |
|35 |53 |y or Y   |
|36 |54 |z or Z   |
|37 |55 |ア or あ   |
|38 |56 |イ or い   |
|39 |57 |ウ or う   |
|3A |58 |エ or え   |
|3B |59 |オ or お   |
|3C |60 |カ or か   |
|3D |61 |キ or き   |
|3E |62 |ク or く   |
|3F |63 |ケ or け   |
|40 |64 |コ or こ   |
|41 |65 |サ or さ   |
|42 |66 |シ or し   |
|43 |67 |ス or す   |
|44 |68 |セ or せ   |
|45 |69 |ソ or そ   |
|46 |70 |タ or た   |
|47 |71 |チ or ち   |
|48 |72 |ツ or つ   |
|49 |73 |テ or て   |
|4A |74 |ト or と   |
|4B |75 |ナ or な   |
|4C |76 |ニ or に   |
|4D |77 |ヌ or ぬ   |
|4E |78 |ネ or ね   |
|4F |79 |ノ or の   |
|50 |80 |ハ or は   |
|51 |81 |ヒ or ひ   |
|52 |82 |フ or ふ   |
|53 |83 |ヘ        |
|54 |84 |ホ or ほ   |
|55 |85 |マ or ま   |
|56 |86 |ミ or み   |
|57 |87 |ム or む   |
|58 |88 |メ or め   |
|59 |89 |モ or も   |
|5A |90 |ヤ or や   |
|5B |91 |ユ or ゆ   |
|5C |92 |ヨ or よ   |
|5D |93 |ラ or ら   |
|5E |94 |リ or り   |
|5F |95 |ル or る   |
|60 |96 |レ or れ   |
|61 |97 |ロ or ろ   |
|62 |98 |ワ or わ   |
|63 |99 |ヰ        |
|64 |100|ヱ        |
|65 |101|ヲ or を   |
|66 |102|ン or ん   |
|67 |103|б or Б   |
|68 |104|в or В   |
|69 |105|г or Г   |
|6A |106|д or Д   |
|6B |107|ж or Ж   |
|6C |108|з or З   |
|6D |109|и or И   |
|6E |110|л or Л   |
|6F |111|м or М   |
|70 |112|н or Н   |
|71 |113|п or П   |
|72 |114|у or У   |
|73 |115|ф or Ф   |
|74 |116|ц or Ц   |
|75 |117|ч or Ч   |
|76 |118|ш or Ш   |
|77 |119|щ or Щ   |
|78 |120|ъ or Ъ   |
|79 |121|ы or Ы   |
|7A |122|ь or Ь   |
|7B |123|э or Э   |
|7C |124|ю or Ю   |
|7D |125|я or Я   |
|7E |126|β or Β   |
|7F |127|γ or Γ   |
|80 |128|δ or Δ   |
|81 |129|ζ or Ζ   |
|82 |130|η or Η   |
|83 |131|θ or Θ   |
|84 |132|ι or Ι   |
|85 |133|λ or Λ   |
|86 |134|μ or Μ   |
|87 |135|ν or Ν   |
|88 |136|ξ or Ξ   |
|89 |137|π or Π   |
|8A |138|σ or Σ   |
|8B |139|τ or Τ   |
|8C |140|υ or Υ   |
|8D |141|φ or Φ   |
|8E |142|χ or Χ   |
|8F |143|ψ or Ψ   |
|90 |144|ω or Ω   |
|91 |145|ა        |
|92 |146|ბ        |
|93 |147|გ        |
|94 |148|დ        |
|95 |149|ე        |
|96 |150|ვ        |
|97 |151|ზ        |
|98 |152|თ        |
|99 |153|ი        |
|9A |154|ლ        |
|9B |155|მ        |
|9C |156|ნ        |
|9D |157|ო        |
|9E |158|პ        |
|9F |159|ჟ        |
|A0 |160|რ        |
|A1 |161|ს        |
|A2 |162|ტ        |
|A3 |163|უ        |
|A4 |164|ფ        |
|A5 |165|ქ        |
|A6 |166|ღ        |
|A7 |167|ყ        |
|A8 |168|შ        |
|A9 |169|ჩ        |
|AA |170|ც        |
|AB |171|ძ        |
|AC |172|წ        |
|AD |173|ჭ        |
|AE |174|ხ        |
|AF |175|ჯ        |
|B0 |176|ჰ        |
|B1 |177|ա or Ա   |
|B2 |178|բ or Բ   |
|B3 |179|գ or Գ   |
|B4 |180|դ or Դ   |
|B5 |181|ե or Ե   |
|B6 |182|զ or Զ   |
|B7 |183|է or Է   |
|B8 |184|Ը or ը   |
|B9 |185|թ or Թ   |
|BA |186|ժ or Ժ   |
|BB |187|ի or Ի   |
|BC |188|լ or Լ   |
|BD |189|խ or Խ   |
|BE |190|ծ or Ծ   |
|BF |191|կ or Կ   |
|C0 |192|հ or Հ   |
|C1 |193|ձ or Ձ   |
|C2 |194|ղ or Ղ   |
|C3 |195|ճ or Ճ   |
|C4 |196|մ or Մ   |
|C5 |197|յ or Յ   |
|C6 |198|ն or Ն   |
|C7 |199|շ or Շ   |
|C8 |200|ո or Ո   |
|C9 |201|չ or Չ   |
|CA |202|պ or Պ   |
|CB |203|ջ or Ջ   |
|CC |204|ռ or Ռ   |
|CD |205|ս or Ս   |
|CE |206|վ or Վ   |
|CF |207|տ or Տ   |
|D0 |208|ր or Ր   |
|D1 |209|ց or Ց   |
|D2 |210|ւ or Ւ   |
|D3 |211|փ or Փ   |
|D4 |212|ք or Ք   |
|D5 |213|ֆ or Ֆ   |
|D6 |214|և        |
|D7 |215|─ or │   |
|D8 |216|┌ or ┐   |
|D9 |217|└ or ┘   |
|DA |218|├ or ┤   |
|DB |219|┬ or ┴   |
|DC |220|┼        | 
|DD |221|╭ or ╮   |
|DE |222|╰ or ╯   |
|FF |255|Unknown  |
