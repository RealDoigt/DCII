# DCII
Doigt's Code of Information Interchange is Doigt's own personal standard for written text on old machines that don't have an official standard for text encoding or for use cases which require supporting more than one alphabet. I don't care about your opinion if your opinion is "this shouldn't exist".

## Advantages

* Lightweight: The character values can be stored in 8-bit values.
* International: It supports multiple writing systems.
* Compact: With the special Uppercase character, we can still have lower and upper case characters while supporting many alphabets and having the lowest possible size for a single character.
* Adaptable: 40 characters reserved for private use, which should give enough breathing room for special use cases.

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
|69 |105|д or Д   |
|6A |106|ж or Ж   |
|6B |107|з or З   |
|6C |108|и or И   |
|6D |109|л or Л   |
|6E |110|м or М   |
|6F |111|н or Н   |
|70 |112|п or П   |
|71 |113|у or У   |
|72 |114|ф or Ф   |
|73 |115|ц or Ц   |
|74 |116|ч or Ч   |
|75 |117|ш or Ш   |
|76 |118|щ or Щ   |
|77 |119|ъ or Ъ   |
|78 |120|ы or Ы   |
|79 |121|ь or Ь   |
|7A |122|э or Э   |
|7B |123|ю or Ю   |
|7C |124|я or Я   |
|7D |125|β or Β   |
|7E |126|γ or Γ   |
|7F |127|δ or Δ   |
|80 |128|ζ or Ζ   |
|81 |129|η or Η   |
|82 |130|θ or Θ   |
|83 |131|ι or Ι   |
|84 |132|λ or Λ   |
|85 |133|μ or Μ   |
|86 |134|ν or Ν   |
|87 |135|ξ or Ξ   |
|88 |136|π or Π   |
|89 |137|σ or Σ   |
|8A |138|τ or Τ   |
|8B |139|υ or Υ   |
|8C |140|φ or Φ   |
|8D |141|χ or Χ   |
|8E |142|ψ or Ψ   |
|8F |143|ω or Ω   |
|90 |144|ა        |
|91 |145|ბ        |
|92 |146|გ        |
|93 |147|დ        |
|94 |148|ე        |
|95 |149|ვ        |
|96 |150|ზ        |
|97 |151|თ        |
|98 |152|ი        |
|99 |153|ლ        |
|9A |154|მ        |
|9B |155|ნ        |
|9C |156|ო        |
|9D |157|პ        |
|9E |158|ჟ        |
|9F |159|რ        |
|A0 |160|ს        |
|A1 |161|ტ        |
|A2 |162|უ        |
|A3 |163|ფ        |
|A4 |164|ქ        |
|A5 |165|ღ        |
|A6 |166|ყ        |
|A7 |167|შ        |
|A8 |168|ჩ        |
|A9 |169|ც        |
|AA |170|ძ        |
|AB |171|წ        |
|AC |172|ჭ        |
|AD |173|ხ        |
|AE |174|ჯ        |
|AF |175|ჰ        |
|B0 |176|ա or Ա   |
|B1 |177|բ or Բ   |
|B2 |178|գ or Գ   |
|B3 |179|դ or Դ   |
|B4 |180|ե or Ե   |
|B5 |181|զ or Զ   |
|B6 |182|է or Է   |
|B7 |183|Ը or ը   |
|B8 |184|թ or Թ   |
|B9 |185|ժ or Ժ   |
|BA |186|ի or Ի   |
|BB |187|լ or Լ   |
|BC |188|խ or Խ   |
|BD |189|ծ or Ծ   |
|BE |190|կ or Կ   |
|BF |191|հ or Հ   |
|C0 |192|ձ or Ձ   |
|C1 |193|ղ or Ղ   |
|C2 |194|ճ or Ճ   |
|C3 |195|մ or Մ   |
|C4 |196|յ or Յ   |
|C5 |197|ն or Ն   |
|C6 |198|շ or Շ   |
|C7 |199|ո or Ո   |
|C8 |200|չ or Չ   |
|C9 |201|պ or Պ   |
|CA |202|ջ or Ջ   |
|CB |203|ռ or Ռ   |
|CC |204|ս or Ս   |
|CD |205|վ or Վ   |
|CE |206|տ or Տ   |
|CF |207|ր or Ր   |
|D0 |208|ց or Ց   |
|D1 |209|ւ or Ւ   |
|D2 |210|փ or Փ   |
|D3 |211|ք or Ք   |
|D4 |212|ֆ or Ֆ   |
|D5 |213|և        |
|FF |255|Unknown  |