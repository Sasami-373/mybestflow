<script>mermaid.initialize({startOnLoad:true});</script>

```mermaid
flowchart TB
  S((start)) -.- a
　
subgraph  
  a{{タイトル精査ステータス確認}}:::className1 -.- b
click a "https://my-best.zendesk.com/hc/ja/articles/6082062393743-%E7%B2%BE%E6%9F%BB%E6%B8%88%E3%81%BF%E3%81%AE%E3%82%BF%E3%82%A4%E3%83%88%E3%83%AB%E3%81%AE%E7%A2%BA%E8%AA%8D"
  b{精査済みタイトル?} -.- |はい| c
  b -.- |いいえ| d
x([タイトル精査について知る]):::className2
click x "https://my-best.zendesk.com/hc/ja/articles/6367885677711-%E3%82%BF%E3%82%A4%E3%83%88%E3%83%AB%E7%B2%BE%E6%9F%BB%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6%E7%9F%A5%E3%82%8B"
end
subgraph  
  c{{タイトル精査シートの入力}}:::className1 -.- e
click c "https://my-best.zendesk.com/hc/ja/articles/6305840743439-%E3%82%BF%E3%82%A4%E3%83%88%E3%83%AB%E7%B2%BE%E6%9F%BB%E3%82%B7%E3%83%BC%E3%83%88%E3%81%AE%E5%85%A5%E5%8A%9B"
  d{{タイトル精査依頼}}:::className1  -.- e
click d "https://my-best.zendesk.com/hc/ja/articles/6305934764047-%E3%82%BF%E3%82%A4%E3%83%88%E3%83%AB%E7%B2%BE%E6%9F%BB%E4%BE%9D%E9%A0%BC"
  e{{全体シートへの着手情報入力}}:::className1 -.- f
click e "https://my-best.zendesk.com/hc/ja/articles/6305953642511-%E5%85%A8%E4%BD%93%E3%82%B7%E3%83%BC%E3%83%88%E3%81%B8%E3%81%AE%E7%9D%80%E6%89%8B%E6%83%85%E5%A0%B1%E5%85%A5%E5%8A%9B"
y([着手連絡について知る]):::className2
click y "https://my-best.zendesk.com/hc/ja/articles/6368161917327"
end
  f{{関係部署へ着手連絡}}:::className1 -.- g
click f "https://my-best.zendesk.com/hc/ja/articles/6305964214671-%E9%96%A2%E4%BF%82%E9%83%A8%E7%BD%B2%E3%81%B8%E7%9D%80%E6%89%8B%E9%80%A3%E7%B5%A1"
  g{モノorサービス}  -.-  |モノ| h
  g -.- |サービス| i
  h[事前商品選定]-.-t
  t[購買申請]-.-p
  p{今日手に入れたい?}  -.-  |はい| q
  p -.- |いいえ| s
  q[店頭購入]  -.-  i
  s[調達依頼]  -.-  i
  i{タイトル精査シートに記事IDはある?} -.- |ある| j
  i -.- |ない| k
  k{カテゴリ一覧に適したカテゴリはある?}  -.-  |ある| l
  k -.- |ない| m
  j[再編集コンテンツページの作成] -.- n
  l[カテゴリの選択] -.- n
  m[新規カテゴリの作成依頼] -.- n
  n[担当者の設定] -.- o
  o[企画書作成]

%% class definitions
    classDef className1 fill:#02bb80,stroke:#999999,stroke-width:0.5px,color:#fff
    classDef className2 fill:#666666,stroke:#999999,stroke-width:0px,color:#fff
