動かせました:+1:
注意点は以下ですかね〜(多分1つ目が重要)

- python-dotenvのバージョン(Renderのpipは20.1.1なので1.0.0は入れれない)
    - 入れる → pip install 'python-dotenv<1' 環境変数用ファイルが使える
    - 入れない → 環境変数を設定すればOK
- RenderのStart Commandはgunicornだと動かない？ 原因分からない
    - [x] `uvicorn ai_talk:app --host 0.0.0.0 --port 10000` OK
    - [ ] `gunicorn ai_talk:app` NG TypeError: __call__() missing 1 required positional argument: 'send'

