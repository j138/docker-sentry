# 動かし方

はじめに、sentry.ymlのメール設定などを見直してください
それから下記コマンドを実行

```
docker-compose up -d redis postgres sentry
docker-compose run sentry upgrade
docker-compose up -d
docker stop sentry_sentry_run_1
curl http://localhost/auth/login/sentry/
```
