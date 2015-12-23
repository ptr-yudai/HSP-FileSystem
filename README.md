HSP-FileSystem
====

Overview
HSP言語でファイルシステムを扱うためのモジュール。
ディスク上のファイルを読み取り、削除されたファイルを復元することを目的とする。

## Requirement
言語 : Hot Soup Processor 3.0以降
ファイルシステム : NTFS

## Usage
ソースコードの先頭に
    #include "mod_Disk_Reader.hsp"
と記述するとディスクアクセスおよびパーティションテーブルの読み込みをするための関数等が使用可能になる。
    #include "mod_NTFS_Parser.hsp"
と記述するとNTFSを解析する各種関数等が使用可能になる。
関数の取り扱いについては各モジュールのコードを参照すること。
モジュール変数(構造体)は全て
    st_構造体名
という名前が使われる。
    st_構造体名_GET
で構造体のデータを取得する。
データが4バイト以内のものについては値を返すが、そうでないものに関してはデータのポインタを返す。

## Licence

改造等自由

## Author

[ptr-yudai] (https://github.com/ptr-yudai)
