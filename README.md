# hello-manifest

1. `helm lint .`
1. tgz生成 `helm package .`
1. index.yaml 生成 `helm repo index .`
1. Webサーバで公開 ` docker run --name nginx -v $PWD:/usr/share/nginx/html -p 8080:80 nginx`
1. リポジトリ追加 `helm repo add local http://IP:Port`
1. helm install local/tamura-app --generate-name