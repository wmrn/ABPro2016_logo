# ABPro2016_logo
ABPro2016のロゴ 2016/09/29  

## そもそも...
ABProのロゴを募集してた。でも、「ABproは普通じゃないプログラミングの発表なので普通じゃないロゴを募集します」といわれた。  
とりあえず普通じゃないなら読めなくしてしまえと思ってグリッチをした。でも読めなさ過ぎて却下。  
ならどうやって普通じゃない感じを出せばいいのか。フォレンジックかな？頭によぎった。  
作ろうとしたがいいアイデアなくてABpro発表に間に合わず。  
今頃になってしまったが作りたかったから作った。  

## 説明
まず、画像にexif情報を付け加えた。  
開催場所の緯度・軽度、作成された時間を会場時間、最終更新時間？を終了時間に編集。  
<img src="https://github.com/wmrn/ABPro2016_logo/blob/master/data/exif.png" title="exif" width="322" height="432" />  
次に画像のバイナリデータの後ろにProcessingのファイルをzipで圧縮させたバイナリを付加する。  
これはctf4gで教えていただいたものを採用した。  
＜参考＞<http://hp.vector.co.jp/authors/VA032610/JPEGFormat/StructureOfJPEG.htm>  
Processingのファイルの中身はABpro2016が行われていた時間にはロゴがパリピな雰囲気を出しながら回転する。  
それ以外の時間では真っ暗の中スポットライトで照らされる。  
時間操作はPCの日付を変更させるか、コードを書き換えればいい。  
<img src="https://github.com/wmrn/ABPro2016_logo/blob/master/data/ABPro2016_off.gif" title="OFF" width="320" height="240" />
<img src="https://github.com/wmrn/ABPro2016_logo/blob/master/data/ABPro2016_on.gif" title="ON" width="320" height="240" />  

## Memo
* メタセコイアで作ったものはライブラリの関係で1系でしか動かない。  
そして、1系で3Dを扱うときの回転軸の指定とかもろもろ面倒くささを感じた。  
Processingは2系が1番いい。(個人の意見)  
Blenderのバージョン注意。  

*  バイナリの構造がJPEGよりもPNGのほうが単純。(教えていただいた。)  
でもだからと言って単純には思うようにずれるわけでもなく、思うように色が変わるわけでもない。  
まだましだった程度。(私が考えるのをあきらめたから)  
いい感じの画像が生成されるまでひたすらやるのは大変だった。  

## 最後に
Blenderの基本の操作とProcessingで３Dモデルを扱う方法をだいぶ学べた。  
今年ABProでるぞとか言ってたのに疲れてアイデアでなくて...そんな言い訳していいわけ？はい。  
