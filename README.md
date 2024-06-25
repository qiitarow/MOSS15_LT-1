# MOSS15 LT#1 資料

[第15回　医療オープンソース協議会](https://moss.connpass.com/event/315545/)　LT#1 資料

タイトル　「HAPI FHIR Starter ProjectのJPAサーバにJP_CoreのIGをインストールする」


環境

* Visual Studio Code
* git
* docker or finch



解説

* HAPI FHIR Starter ProjectのApplication.yamlを修正し、JP Core IGがインストールされた状態で、Dockerコンテナ上にサーバを立ち上げます。
* Application.yaml内に解説があります。
* postgressをデータベースに指定したdockerの構成です。
* hapi-extra-classesディレクトリはカスタマイズのためのインターセプターを置く場所です。（現在は空です。）
* docker（ここでは、finchを利用）でコンテナを立ち上げます。



コマンド例

```
> mkdir HAPI_FHIR_STARTER
> cd HAPI_FHIR_STARTER
> mkdir hapi-extra-classes
> git clone https://github.com/qiitarow/MOSS15-LT-1.git
> finch compose up
```



リンク

[HAPI FHIR](https://hapifhir.io/hapi-fhir/)

[HAPI FHIR Starter Project](https://github.com/hapifhir/hapi-fhir-jpaserver-starter.git)
