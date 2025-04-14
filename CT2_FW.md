# CT2 の FW 調整

端末に合わせて、以下のファイルをダウンロードします。

### TAB-A03-BS

[**recovery-a03bs.zip**](https://github.com/s1204IT/CPadGmsSystem/releases/download/latest/recovery-a03bs.zip)

### TAB-A03-BR/BR2/BR2B

[**recovery-a03br2.zip**](https://github.com/s1204IT/CPadGmsSystem/releases/download/latest/recovery-a03br2.zip)

ダウンロードしたら展開し、`recovery-a03**.img` を **Rufus** 等を用いてSDカードにフラッシュします。

端末のシャットダウンし、SDカードを挿入したら、リカバリーから初期化する動作を実行します。  
参考：<https://www.benesse.co.jp/member/helpdesk/close/process.html>

すると、ファームウェアアップデートが自動的に始まるので、端末に触れずに完了するまで待ちます。

再起動後、ビルド番号が次の通りになっていれば成功です。

- **TAB-A03-BS**：`01.16.000`
- **TAB-A03-BR/BR2/BR2B**：`02.04.000`

---

[**ここ**](CT2.md)から処理を続行してください。
