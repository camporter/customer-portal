---

copyright:

  years: 1994, 2018

lastupdated: "2018-02-12"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 環境およびシステム・イベントのモニタリング
{: #customerportal_cpmonenvsysevent}

環境をモニターするということは、いつでもデバイスをチェックできること、および、デバイスの 1 つがダウンした場合に自動的に通知されることを意味します。 システムが円滑に稼働している状態を保つためにシステム・イベントをモニターすることもできます。  
{: shortdesc}

## 環境のモニタリング
{: #cpmonenv}

最低限、基本的な ping モニタリングを使用しますが、業務上のニーズに最も適合するようにモニタリング・オプションをカスタマイズできます。 モニタリング・オプションについては、[ベア・メタル・サーバーのセットアップ](/docs/customer-portal/cpsetupbaremetal.html)を参照してください。

### ネットワーク保守および予定外のイベントの情報を常に入手する
{: #cp_stayinfomaintevent}

スケジュールされた緊急ネットワーク保守が不可避であることが時々あります。 {{site.data.keyword.BluSoftlayer_full}} インフラストラクチャーは、スケジュールされた緊急時保守イベントのすべての情報をユーザーが常に入手できるように、[Twitter アカウント ![外部リンク・アイコン](../icons/launch-glyph.svg)](https://twitter.com/softlayernotify){:new_window} など、多くのチャネルを保守します。 さらに、Event Management System からの [E メール通知をサブスクライブする](/docs/customer-portal/cpsub2not.html)こともできます。 この無料サービスは、各種サービスに影響を与える可能性のある予定外のイベントに関して、サブスクライブしたユーザーに自動的に E メールを送信します。

### {{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・モバイルを使用する
{: #cp_bmxinframobile}

{{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・モバイルを使用して、iOS または Android モバイル・デバイスを使用する持ち運べる {{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・デバイスを管理します。 {{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・モバイルの機能には、チケット作成のサポート、基本的なデバイス制御、および処理能力モニタリングが含まれます。

{{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・モバイル・アプリケーションは、カスタマー・ポータルの機能を補完します。ユーザーはネットワーク接続されたモバイル・デバイスを使用してどこからでもインフラストラクチャーに関する重要な情報をモニターすることができます。このアプリケーションは急速に進化し、定期的に新しい機能が追加されていますが、ユーザーはモバイル・アプリケーションを使用して以下のようなタスクを実行できます。
  * サポート・チケットの表示、作成、および更新
  * 処理能力やアラームを含めたデバイス状況のモニター
  * ベア・メタル・サーバーおよび仮想サーバーのシャットダウンと再始動
  * アカウントの請求書の表示、および 1 回限りの支払いの実行
  * オブジェクト・ストレージに保管されたコンテンツのアクセスと検査

{{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・モバイル・アプリケーションは、よく使用されている複数のモバイル・デバイス・プラットフォームで使用可能であり、各プラットフォームの関連アプリケーション・ストアから無料で入手できます。

## システム・イベントのモニタリング
{: #customerportal_monevent}

監査ログおよびアクセス・ログを表示することによって、システム・イベントをモニターできます。

### アカウントの監査ログを表示する
{: #cp_viewacctauditlog}

各カスタマー・ポータル・アカウントには、カスタマー・ポータル内の各ユーザーの対話をトラッキングする監査ログが付属しています。 トラッキングされる対話には、ログイン試行 (成功および失敗)、ポート速度の更新、電源オン/オフおよびリブート、および、{{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・サポート担当員によって行われる対話が含まれます。 ユーザー・アカウントの監査ログを表示するには、以下の手順を使用します。

1. 固有の資格情報を使用して[カスタマー・ポータル ![外部リンク・アイコン](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} にアクセスします。
2. ナビゲーション・バーから**「アカウント」** > **「管理」** > **「監査ログ (Audit Log)」**を選択して、監査ログにアクセスします。

最初は、監査ログでは、アカウントのユーザーによって行われた最後の 25 個の対話が表示されます。 200 個までの対話をいつでも表示できます。 表示される結果の数は**「表示 (Display)」**ドロップダウン・リストで更新できます。 設定が変更された場合、対話の**「アクション (Action)」**列にリンクが含まれます。 任意のリンクをクリックすると、アクションの影響を受ける設定と、変更の詳細が表示されます。 任意の対話のデバイス名またはユーザー名をクリックすると、それぞれ、デバイス詳細画面またはユーザー・プロファイル画面にリダイレクトされます。

### ユーザーのアクセス・ログを表示する
{: #cp_viewuserlogs}

アクセス・ログでは、特定のカスタマー・ポータル・ユーザーによって行われた各アクセス試行のデータが示されます。 このログでは、各アクセス試行の日時スタンプ、および IP アドレスが示されます。 ユーザーのアクセス・ログを表示するには、以下の手順を使用します。

1. 固有の資格情報を使用して[カスタマー・ポータル ![外部リンク・アイコン](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} にアクセスします。
2. メニュー・バーから**「アカウント」** > **「ユーザー」**を選択して、「ユーザー」ウィンドウにアクセスします。
3. **「アクション (Actions)」**ドロップダウン・リストから**「監査ログの表示 (View Audit Log)」**を選択して、ユーザーのアクセス・ログを表示します。

各ユーザーのアクセス・ログでは、そのユーザーによって行われたアクセス試行が、日付別に、アクセス試行が行われた IP アドレスと共に示されます。 アクセス・ログ内の情報は読み取り専用であり、どのようなときでも内容を編集することはできません。 上の手順を繰り返すことによって、いつでもアクセス・ログを再表示できます。 ログを終了して「ユーザー」画面に戻るには、画面の上部にある**「すべてのユーザーの表示 (View All Users)」**リンクをクリックします。