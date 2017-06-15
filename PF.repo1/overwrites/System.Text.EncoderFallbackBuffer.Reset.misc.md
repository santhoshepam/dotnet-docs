---
uid: System.Text.EncoderFallbackBuffer.Reset
additional_notes.overrides: *content
---

<p>After calling the <xref href="System.Text.EncoderFallbackBuffer.Reset"></xref> method, the <xref href="System.Text.EncoderFallbackBuffer.Remaining"></xref> property should return 0, the <xref href="System.Text.EncoderFallbackBuffer.GetNextChar"></xref> method should return U+0000, and the <xref href="System.Text.EncoderFallbackBuffer.MovePrevious"></xref> method should return `false`.</p>


