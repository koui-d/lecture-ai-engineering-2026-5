# 第6回 解答

## 演習

<!-- [tool call] の行は、表示された行をそのまま貼り付けてください。終わらなかった STEP は、空欄のままでかまいません。 -->

- STEP 1 のツールの名前：
[search_materials]
- STEP 2 の [tool call]：
[tool call]   glossary_search_glossary({'query': '3レベル'})
- STEP 3 の [tool call]：
[tool call]   fetch_fetch({'url': 'https://modelcontextprotocol.io/'})
- STEP 4 の [tool call]：
[tool call]   aws_aws___search_documentation({'topics': ['general'], 'search_phrase': 'Amazon S3 バージョニング 概要'})
- 気づき・疑問：
・uv run python -m app.mcp_agent --traceの指示は同じだが、fetch,awsと増やしていくことで[server]が一つずつ増えるのはわかるが、[tools] MCP サーバー（app/mcp_servers.json）は同じなのにどうして[tool call]が変わるのかが疑問だ。
・最後にuv run python -m app.mcp_agent --trace "AIE2026の講座の宿題にある「3レベル」とは何ですか？"をもう一度実行すると、きちんとglossary_search_glossaryが答えた。ここでしかわからない知識なので正しい[tool call] の選択ができている。

## 宿題

<!-- 基礎・実装・発展のどれか1つに取り組めば完了です。 -->

- 取り組んだレベル：基礎 
- やったこと：mcpサーバーにget_lecture_summaryを追加する。
- 結果：
- 気づき・疑問：
