# プロジェクト全体のフォルダ

## 使い方
 ### ①git cloneフォークして自分のリポジトリをクローンする　git clone　URL

### ルートディレクトリに移動
 ### cd ディレクトリ名
 ### git submodule init  
 ### git submodule update　サブモジュール（フロント、バックエンドを最新化する）

 ### Docker Desktopを起動する
![docker](https://github.com/user-attachments/assets/68dcb70f-2e89-40bc-9dbe-5a15664022d9)


 ### ③docker-compose.ymlがあるディレクトリでターミナルからdocker-compose up -dで実行

 ### ④モジュールのインストールがある場合はvolumeを削除かも（未確認）　docker-compose down --volumes

 front側にnode_modulesが入っていないとエラーになることがある。
 下のコマンドを打つってnode_modulesを入れる
 cd healthcare_front 
 npm install 

データベースがつかないと、Djangoがつかないので先にデータベースを起動する。ß

このような画面になればOK
 ![docker2](https://github.com/user-attachments/assets/f28eb80b-434b-4c22-ade7-35ca0645fdcc)

portの3000 や8000をクリックすると実行中の画面にアクセスできる。


Djangoは画面を更新すると更新が反映される
reactはdockerの再起動を行ったら反映されたため時間がかかった→ホットリロードの方法はあるみたい