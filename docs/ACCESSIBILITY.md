# Accessibility

Last updated: 2026-11-26

## Priorities and Goals

This statement covers:

- The UI of Gemini Scraping Code Generator (`gemini-scraping-code-generator.html`, including the version published on GitHub Pages)

For the UI, we target WCAG 2.2 Level AA, and we treat it as a minimum, not a ceiling. Some of our own rules are stricter than AA (see [Contributor Expectations](#contributor-expectations)).

## Supported Environments

- Browser: Tested with Chrome and Edge. Not yet tested with Firefox or Safari
- Operating systems: Tested on Windows. Not yet tested on macOS, Linux, iOS, or Android
- Screen readers: Tested with NVDA and Narrator. Not yet tested with PC-Talker, JAWS, VoiceOver, or TalkBack

## Known Limitations

- The accessibility of the generated Python code, and of the HTML file that code produces, depends on Gemini's output. The tool asks Gemini for dark theme support, sufficient contrast, and a minimum font size, but the output does not always meet them. These requirements (such as 4.5:1 or higher for text) are also looser than the rules for this tool's own UI. Please check the generated HTML before you use it

## Reporting Accessibility Barriers

Please report barriers through [GitHub Issues](https://github.com/securecat/gemini-scraping-code-generator/issues). You can write in English or Japanese.

The following details help us, but all of them are optional:

- What you were trying to do
- The screen or feature you were using
- What happened, and what you expected
- Your OS, browser version, and Gemini Scraping Code Generator version
- Any assistive technology you use, such as a screen reader

You don't need to tell us about any disability. Screenshots and recordings are not required.

## Response Process

Gemini Scraping Code Generator is developed by an individual, so we can't promise a deadline for replies or fixes. We will respond as quickly as we can.

- We will reply on the issue once we've seen your report
- If there is a workaround, we will share it
- Before releasing a fix, we may ask you to confirm that it works for you
- Fixes are recorded in the [commit history](https://github.com/securecat/gemini-scraping-code-generator/commits/main)

## Contributor Expectations

These expectations apply equally to human contributors and coding agents.

When you change the UI:

- Use native form controls (`<input>`, `<select>`, `<textarea>`). Don't use `<div>` or `<span>` as buttons; use `<button>` for actions on the page and `<a>` for navigation
- Don't use the `disabled` attribute
- Don't remove focus indicators (no `outline: none`)
- Don't remove link underlines
- Keep text contrast at 7:1 or higher for body text and 4.5:1 or higher for secondary text, in both light and dark themes
- Keep non-text elements, such as borders and icons, at 3:1 or higher against adjacent colors
- Don't apply `opacity` to elements that need contrast
- Use a minimum font size of 16px for Japanese and 14px for English
- Use `font-family: sans-serif` (don't use `system-ui`)
- Don't dismiss status messages automatically
- Don't add anything that moves on its own, such as auto-scrolling

After the change, check that everything can be operated with a keyboard alone, and that a screen reader reads the content correctly.

The prompt sent to Gemini includes accessibility requirements for the generated HTML. When you change the prompt, don't loosen these requirements.

## Ownership and Maintenance

This statement is maintained by the maintainer, securecat. We update it when we add features or when the tested environments change.

## Feedback on This Statement

Suggestions about this statement or our approach to accessibility are also welcome through [GitHub Issues](https://github.com/securecat/gemini-scraping-code-generator/issues).

---

# アクセシビリティ

最終更新：2026-11-26

## 優先事項と目標

この文書が対象とするのは、次のとおりです。

- Gemini スクレイピングコード・ジェネレーターの画面（`gemini-scraping-code-generator.html`。GitHub Pages で公開しているものを含む）

UIは WCAG 2.2 のレベル AA を目標とし、これを上限ではなく下限と考えています。AAより厳しい独自の基準もあります（[貢献者への期待](#貢献者への期待)を参照）。

## 対応している環境

- ブラウザ：Chrome、Edge で確認済み。Firefox、Safari はまだ試していません
- OS：Windows で確認済み。macOS、Linux、iOS、Android はまだ試していません
- スクリーンリーダー：NVDA、ナレーターで確認済み。PC-Talker、JAWS、VoiceOver、TalkBack はまだ試していません

## 既知の制限

- 生成される Python コードと、そのコードが出力する HTML ファイルのアクセシビリティは、Gemini の出力によって変わります。ダークテーマへの対応、コントラスト比、文字サイズを Gemini に指示していますが、毎回満たされるとは限りません。また、この指示の基準（テキストは 4.5:1 以上など）は、このツール自身の画面の基準より緩いものです。生成された HTML は、使う前に確認してください

## アクセシビリティの問題を報告する

問題は [GitHub Issues](https://github.com/securecat/gemini-scraping-code-generator/issues) で報告してください。日本語でも英語でも構いません。

次のことを書いてもらえると助かりますが、どれも任意です。

- 何をしようとしていたか
- 使っていた画面や機能
- 何が起きたか、どうなると思っていたか
- OS、ブラウザのバージョン、Gemini スクレイピングコード・ジェネレーターのバージョン
- 使っている支援技術（スクリーンリーダーなど）

障害の有無や内容を書く必要はありません。スクリーンショットや録画も必須ではありません。

## 対応の流れ

Gemini スクレイピングコード・ジェネレーターは個人で開発しているため、返信や修正の期限はお約束できません。それでも、できるかぎり早く対応します。

- 報告を確認したら、Issue で返信します
- 回避策があれば、お知らせします
- 修正をリリースする前に、問題が解消したかどうかの確認をお願いすることがあります
- 修正の内容は [コミット履歴](https://github.com/securecat/gemini-scraping-code-generator/commits/main) に記録します

## 貢献者への期待

ここに挙げることは、人間の貢献者にもコーディングエージェントにも、同じように求めます。

UIを変更するときは、次を守ってください。

- フォームにはネイティブの要素（`<input>`・`<select>`・`<textarea>`）を使う。`<div>` や `<span>` をボタンの代わりにしない。画面内の操作には `<button>`、ページの移動には `<a>` を使う
- `disabled` 属性を使わない
- フォーカスインジケーターを消さない（`outline: none` を使わない）
- リンクの下線を消さない
- テキストのコントラスト比は、本文で 7:1 以上、補足的なテキストで 4.5:1 以上にする。ライトテーマとダークテーマのそれぞれで満たす
- 境界線やアイコンなど、テキスト以外の要素も、隣り合う色に対して 3:1 以上にする
- コントラストが必要な要素に `opacity` を使わない
- 文字サイズは、日本語で 16px 以上、英語で 14px 以上にする
- `font-family` は `sans-serif` にする（`system-ui` は使わない）
- ステータスメッセージを自動で消さない
- 自動スクロールなど、ひとりでに動くものを作らない

変更したあとは、キーボードだけですべて操作できること、スクリーンリーダーで内容が正しく読み上げられることを確認してください。

Gemini に送るプロンプトには、生成される HTML のアクセシビリティの要件が含まれています。プロンプトを変更するときは、これらの要件を緩めないでください。

## 責任者と保守

この文書は、メンテナーの securecat が管理しています。機能を追加したときや、動作を確認した環境が変わったときに更新します。

## この文書へのフィードバック

この文書やアクセシビリティへの取り組み方についての提案も、[GitHub Issues](https://github.com/securecat/gemini-scraping-code-generator/issues) で受け付けています。
