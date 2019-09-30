---
id: dist
{{if .Meta.Status}}status: {{.Meta.Status}}{{end}}
{{if .Meta.Summary}}summary: {{.Meta.Summary}}{{end}}
{{if .Meta.Author}}author: {{.Meta.Author}}{{end}}
{{if .Meta.Categories}}categories: {{commaSep .Meta.Categories}}{{end}}
{{if .Meta.Tags}}tags: {{commaSep .Meta.Tags}}{{end}}
{{if .Meta.Feedback}}feedback link: {{.Meta.Feedback}}{{end}}
{{if .Meta.GA}}analytics account: {{.Meta.GA}}{{end}}

---

# LINE Pay ハンズオン資料

## 加盟店審査

申請書類の不備などが二度ありましたが、約2週間で審査完了しました。審査がスムーズなのも時間がない個人としてはうれしいところです。

審査が完了すると、下のようなメールが届きます。
![加盟店審査完了メール](images/ReviewCompleted.png)

## LINE Pay Sandboxの申請と設定

実際に決済するには加盟店登録が必要ですが、開発して動作を確認するフェーズであればSandbox が利用できます。こちらは下記のURLから申請すると、Sandbox 用のLINE Pay API アカウントが払い出されますので、誰でもすぐに利用できます。

### LINE Pay Sandboxの申請
    - @<href>{https://pay.line.me/jp/developers/techsupport/sandbox/creation?locale=ja_JP}

アカウントが払い出されたらLINE Pay コンソールの決済連動管理 > 連動キー管理からChannel ID とChannel Secret Key を確認します。これらの値はLINE Pay のAPI コールに必要になります。
![連動キー管理](images/LinkKey.png)
