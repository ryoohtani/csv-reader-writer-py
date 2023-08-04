## Learning Python for the first time
## 初めてのPythonの学習

<sub> Learning to create a Python environment in docker, learning the basics of Python, and creating a function to output csv. We also created an environment to learn how to install flask and fastapi, and only check that they work. </sub>

<sub> Python環境をdocker内に作成するための学習、Pythonの基本を学習し、csvを出力する機能を作成。併せてflaskとfastapiの導入と動作確認のみ行える環境も学習のために行いました。</sub>

**環境構築**

*dockerコマンド*

* ビルドコマンド
```
docker-compose build
```
* 環境の立ち上げ
```
docker-compose up -d
```
* コンテナにアクセス(python-csvはコンテナ名)
```
docker exec -it python-csv /bin/bash
```

*Pythonのコマンド*

* requirements.txt(事前にライブラリやインストールしたいもの記載)
```
pip install -r requirements.txt
```

* set.py(Pythonのパッケージをビルド、インストール、配布する際の必要情報記載)
```
python setup.py sdist
```

FastAPI用のコマンドメモ
* 起動コマンド
```
uvicorn fastapis:app --host 自身で決めたhostの番号 --port 自身で決めたportの番号 
```

*gitコマンド*

* ローカルリポジトリの新規作成
```
git init
```

* ファイルの追跡(変更分全て)
```
git add .
```

* コミット
```
git commit
```

* ローカルリポジトリにリモートリポジトリのURLを貼り付ける
```
git remote add origin URLを貼り付ける
```

* リモートリポジトリへプッシュ
```
git push -u origin main
```