<div class="Box-sc-g0xbh4-0 bJMeLZ js-snippet-clipboard-copy-unpositioned" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">SQLCoder 除雾</font></font></h1><a id="user-content-defog-sqlcoder" class="anchor" aria-label="永久链接：除雾 SQLCoder" href="#defog-sqlcoder"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Defog 的 SQLCoder 是一系列最先进的 LLM，用于将自然语言问题转换为 SQL 查询。</font></font></p>
<p dir="auto"><a href="https://defog.ai/sqlcoder-demo/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">互动演示</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">| </font></font><a href="https://huggingface.co/defog/sqlcoder-7b-2" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">🤗 HF 回购</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">| </font></font><a href="https://colab.research.google.com/drive/1z4rmOEiFkxkMiecAWeTUlPl0OmKgfEu7?usp=sharing" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">♾️ Colab</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> | </font></font><a href="https://twitter.com/defogdata" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">🐦 推特</font></font></a></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">长话短说</font></font></h2><a id="user-content-tldr" class="anchor" aria-label="永久链接：TL;DR" href="#tldr"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">SQLCoder 是一系列大型语言模型，其性能优于</font></font><code>gpt-4</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们的</font><a href="https://github.com/defog-ai/sql-eval"><font style="vertical-align: inherit;">sql-eval</font></a></font><code>gpt-4-turbo</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">框架上的自然语言到 SQL 生成任务</font><font style="vertical-align: inherit;">，并且显着优于所有流行的开源模型。</font></font><a href="https://github.com/defog-ai/sql-eval"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/5008293/303899859-22b891db-2201-4b30-a52d-22376ba8ec86.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQ3OTM5NzIsIm5iZiI6MTcxNDc5MzY3MiwicGF0aCI6Ii81MDA4MjkzLzMwMzg5OTg1OS0yMmI4OTFkYi0yMjAxLTRiMzAtYTUyZC0yMjM3NmJhOGVjODYucG5nP1gtQW16LUFsZ29yaXRobT1BV1M0LUhNQUMtU0hBMjU2JlgtQW16LUNyZWRlbnRpYWw9QUtJQVZDT0RZTFNBNTNQUUs0WkElMkYyMDI0MDUwNCUyRnVzLWVhc3QtMSUyRnMzJTJGYXdzNF9yZXF1ZXN0JlgtQW16LURhdGU9MjAyNDA1MDRUMDMzNDMyWiZYLUFtei1FeHBpcmVzPTMwMCZYLUFtei1TaWduYXR1cmU9YzcxZTQ2NDFjZWFhMDcwNDZjMDA3MzVjODliNjhhODdlNmE2MDM0MDJjNzZkODUyZDI0NzYwZjI5OTUyNjMwOSZYLUFtei1TaWduZWRIZWFkZXJzPWhvc3QmYWN0b3JfaWQ9MCZrZXlfaWQ9MCZyZXBvX2lkPTAifQ.bO5533j1Ggkl1aBuNU27QpxQKxcFY0T5GtFYVvUboXU"><img src="https://private-user-images.githubusercontent.com/5008293/303899859-22b891db-2201-4b30-a52d-22376ba8ec86.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQ3OTM5NzIsIm5iZiI6MTcxNDc5MzY3MiwicGF0aCI6Ii81MDA4MjkzLzMwMzg5OTg1OS0yMmI4OTFkYi0yMjAxLTRiMzAtYTUyZC0yMjM3NmJhOGVjODYucG5nP1gtQW16LUFsZ29yaXRobT1BV1M0LUhNQUMtU0hBMjU2JlgtQW16LUNyZWRlbnRpYWw9QUtJQVZDT0RZTFNBNTNQUUs0WkElMkYyMDI0MDUwNCUyRnVzLWVhc3QtMSUyRnMzJTJGYXdzNF9yZXF1ZXN0JlgtQW16LURhdGU9MjAyNDA1MDRUMDMzNDMyWiZYLUFtei1FeHBpcmVzPTMwMCZYLUFtei1TaWduYXR1cmU9YzcxZTQ2NDFjZWFhMDcwNDZjMDA3MzVjODliNjhhODdlNmE2MDM0MDJjNzZkODUyZDI0NzYwZjI5OTUyNjMwOSZYLUFtei1TaWduZWRIZWFkZXJzPWhvc3QmYWN0b3JfaWQ9MCZrZXlfaWQ9MCZyZXBvX2lkPTAifQ.bO5533j1Ggkl1aBuNU27QpxQKxcFY0T5GtFYVvUboXU" alt="针对训练中未见的新颖模式正确生成 SQL 查询的百分比 (n = 200)，具有 4 个梁 (2)" style="max-width: 100%;"></a></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安装 SQLCoder</font></font></h2><a id="user-content-installing-sqlcoder" class="anchor" aria-label="永久链接：安装 SQLCoder" href="#installing-sqlcoder"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果在配备 NVIDIA GPU 且 VRAM 超过 16GB 的设备上运行（最佳性能）
</font></font><code>pip install "sqlcoder[transformers]"</code></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果在 Apple Silicon 上运行（由于量化和缺乏波束搜索，性能较差）
</font></font><code>CMAKE_ARGS="-DLLAMA_METAL=on" pip install "sqlcoder[llama-cpp]"</code></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果在没有 GPU 访问权限的非苹果芯片计算机上运行，&ZeroWidthSpace;&ZeroWidthSpace;请在 Linux/Intel Mac 上运行
</font></font><code>CMAKE_ARGS="-DLLAMA_BLAS=ON -DLLAMA_BLAS_VENDOR=OpenBLAS" pip install "sqlcoder[llama-cpp]"</code></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">并在 Windows 上运行它</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-smi">$env</span>:CMAKE_ARGS = <span class="pl-s"><span class="pl-pds">"</span>-DLLAMA_BLAS=ON -DLLAMA_BLAS_VENDOR=OpenBLAS<span class="pl-pds">"</span></span>
pip install <span class="pl-s"><span class="pl-pds">"</span>sqlcoder[llama-cpp]<span class="pl-pds">"</span></span></pre><div class="zeroclipboard-container">
   
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">SQLCoder 尚未在其他平台上进行测试。非常欢迎在其他平台上进行测试的贡献！</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">运行 SQLCoder</font></font></h2><a id="user-content-running-sqlcoder" class="anchor" aria-label="永久链接：运行 SQLCoder" href="#running-sqlcoder"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在您的终端中，运行
</font></font><code>sqlcoder launch</code></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">这样，您将能够直接连接到数据库，以便您可以添加元数据并进行可视化查询。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">执照</font></font></h2><a id="user-content-license" class="anchor" aria-label="永久链接：许可证" href="#license"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">此存储库中的代码（内容很少）已获得 Apache-2 许可。模型重量有</font></font><code>CC BY-SA 4.0</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">许可证。总而言之，您可以出于任何目的使用和修改模型 - 包括商业用途。但是，如果您修改权重（例如，通过微调），则必须在相同的许可条款下开源修改后的权重。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">训练</font></font></h2><a id="user-content-training" class="anchor" aria-label="永久链接：培训" href="#training"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Defog 接受了超过 20,000 个人工问题的培训。这些问题基于 10 种不同的模式。训练数据中的任何模式均未包含在我们的评估框架中。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您可以阅读有关我们的</font></font><a href="https://defog.ai/blog/open-sourcing-sqlcoder2-7b/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">培训方法</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><a href="https://defog.ai/blog/open-sourcing-sqleval/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">评估框架</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">的更多信息。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">按问题类别划分的结果</font></font></h2><a id="user-content-results-by-question-category" class="anchor" aria-label="固定链接：按问题类别划分的结果" href="#results-by-question-category"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们将每个生成的问题分为 6 个类别之一。该表显示每个模型正确回答问题的百分比（按类别细分）。</font></font></p>
<table>
<thead>
<tr>
<th></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">日期</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">通过...分组</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">订单依据</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">比率</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">加入</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在哪里</font></font></th>
</tr>
</thead>
<tbody>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">sqlcoder-70b</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">96</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">91.4</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">97.1</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">85.7</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">97.1</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">91.4</font></font></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">sqlcoder-7b-2</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">96</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">91.4</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">94.3</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">91.4</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">94.3</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">77.1</font></font></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">sqlcoder-34b</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">80</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">94.3</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">85.7</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">77.1</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">85.7</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">80</font></font></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">GPT-4</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">72</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">94.3</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">97.1</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">80</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">91.4</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">80</font></font></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">GPT-4-涡轮</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">76</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">91.4</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">91.4</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">62.8</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">88.6</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">77.1</font></font></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">自然 SQL-7b</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">56</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">88.6</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">85.7</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">60</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">88.6</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">80</font></font></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">sqlcoder-7b</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">64</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">82.9</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">74.3</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">54.3</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">74.3</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">74.3</font></font></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">GPT-3.5</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">72</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">77.1</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">82.8</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">34.3</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">65.7</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">71.4</font></font></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">克劳德-2</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">52</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">71.4</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">74.3</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">57.1</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">65.7</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">62.9</font></font></td>
</tr>
</tbody>
</table>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用 SQLCoder</font></font></h2><a id="user-content-using-sqlcoder" class="anchor" aria-label="永久链接：使用 SQLCoder" href="#using-sqlcoder"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您可以通过库使用 SQLCoder，</font></font><code>transformers</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">从 Hugging Face 存储库下载我们的模型权重。我们添加了用于</font></font><a href="/defog-ai/sqlcoder/blob/main/inference.py"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">推断</font></font></a><font style="vertical-align: inherit;"></font><a href="/defog-ai/sqlcoder/blob/main/metadata.sql"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">示例数据库模式</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">的示例代码</font><font style="vertical-align: inherit;">。</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python inference.py -q <span class="pl-s"><span class="pl-pds">"</span>Question about the sample database goes here<span class="pl-pds">"</span></span>

<span class="pl-c"><span class="pl-c">#</span> Sample question:</span>
<span class="pl-c"><span class="pl-c">#</span> Do we get more revenue from customers in New York compared to customers in San Francisco? Give me the total revenue for each city, and the difference between the two.</span></pre><div class="zeroclipboard-container">
    
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><a href="https://defog.ai/sqlcoder-demo" rel="nofollow"><font style="vertical-align: inherit;">您还可以在</font></a><font style="vertical-align: inherit;">我们的网站上使用演示</font></font><a href="https://defog.ai/sqlcoder-demo" rel="nofollow"><font style="vertical-align: inherit;"></font></a></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">硬件要求</font></font></h2><a id="user-content-hardware-requirements" class="anchor" aria-label="永久链接：硬件要求" href="#hardware-requirements"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">SQLCoder-34B 已在带有权重的 4xA10 GPU 上进行了测试</font></font><code>float16</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。您还可以在具有 20GB 或更多内存的消费类 GPU 上加载模型的 8 位和 4 位量化版本 - 例如 RTX 4090、RTX 3090 以及具有 20GB 或更多内存的 Apple M2 Pro、M2 Max 或 M2 Ultra 芯片的记忆。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">去做</font></font></h2><a id="user-content-todo" class="anchor" aria-label="永久链接： 都都" href="#todo"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul class="contains-task-list">
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">开源 v1 模型权重</font></font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用更多数据和更高的数据方差训练模型</font></font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用奖励建模和 RLHF 进一步调整模型</font></font></li>
<li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">从头开始预训练专门用于 SQL 分析的模型</font></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">明星历史</font></font></h2><a id="user-content-star-history" class="anchor" aria-label="永久链接：明星历史" href="#star-history"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><a href="https://star-history.com/#defog-ai/sqlcoder&amp;Date" rel="nofollow"><img src="https://camo.githubusercontent.com/65361ae2fbf958a4fba70f91742a9b55343e40da1697cbeafe33de6936f63308/68747470733a2f2f6170692e737461722d686973746f72792e636f6d2f7376673f7265706f733d6465666f672d61692f73716c636f64657226747970653d44617465" alt="明星历史图" data-canonical-src="https://api.star-history.com/svg?repos=defog-ai/sqlcoder&amp;type=Date" style="max-width: 100%;"></a></p>
</article></div>
