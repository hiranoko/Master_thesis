## Requirement  
Old SAD
X server

## 作業ディレクトリへ移動  
  
<pfrproc1><1:52pm></users/magnet/>cd epics  
<pfrproc1><1:52pm></users/magnet/epics/>cd response/  
<pfrproc1><1:52pm></users/magnet/epics/response/>ls  

## SADの実行と.psへの変換  
  
<pfrproc1><1:52pm></users/magnet/epics/response/>nemacs disp  
<pfrproc1><1:53pm></users/magnet/epics/response/>go v9_16_asym disp  
*** Welcome to SAD Ver.1.0.10.5.6a18 built at 2014-02-13 21:00:09 +0900***  
実行開始  
  
<pfrproc1><1:53pm></users/magnet/epics/response/>ls  
<pfrproc1><1:53pm></users/magnet/epics/response/>tdr fort.12  
<pfrproc1><1:53pm></users/magnet/epics/response/>tdrp fort.12  

## tdr(エイリアス)

<pfrproc1><1:53pm></users/magnet/epics/response/>cat ~/work/tdr  
tdrp* tdrt* tdrx*  
<pfrproc1><1:53pm></users/magnet/epics/response/>cat ~/work/tdr  
cat: /users/magnet/work/tdr: No such file or directory  
<pfrproc1><1:53pm></users/magnet/epics/response/>cat ~/work/tdrp  
td -b -d postscr $1  
mv POSTSCRIPT $1.ps  

## .psの描画on windows 

作成したpsファイルの描画はGoastScriptで確認
pngへの変換は以下の[サイト](https://convertio.co/ja/ps-png/"convertio")とか