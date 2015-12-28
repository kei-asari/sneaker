# サービス概要
>靴（スニーカー）特化型のECサイト。購入動作のみ
>（ユーザーのサイズにマッチするもののみを商品一覧ページで表示したい）
>ユーザーは購入した商品にレビュー（投稿、編集、削除）できる。
>検索機能は諦める。在庫管理システムは今回実装しない。
>テーブルはユーザーテーブルと商品テーブル、中間テーブルとして購入リストテーブルも作成（詳細は後述）


# テーブル設計
##ユーザーテーブル(user)

  １:id
  ２:uesr_name
  ３:mail
  ４:size
  ５:credit_card?
  ６:password


##商品テーブル(product)

  1:id
  2:product_name
  3:price
  4:stock
  5:size

##購入リストテーブル(user_product)

  1:user_id
  2:product_id
  3:buy_date
