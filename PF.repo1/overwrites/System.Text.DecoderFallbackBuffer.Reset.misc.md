---
uid: System.Text.DecoderFallbackBuffer.Reset
additional_notes.overrides: *content
---

<p>After calling the <xref href="System.Text.DecoderFallbackBuffer.Reset"></xref> method, the <xref href="System.Text.DecoderFallbackBuffer.Remaining"></xref> property should return 0, the <xref href="System.Text.DecoderFallbackBuffer.GetNextChar"></xref> method should return U+0000, and the <xref href="System.Text.DecoderFallbackBuffer.MovePrevious"></xref> method should return `false`.</p>


