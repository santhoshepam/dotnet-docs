---
uid: System.Speech.Synthesis.TtsEngine.TtsEngineSsml.Speak(System.Speech.Synthesis.TtsEngine.TextFragment[],System.IntPtr,System.Speech.Synthesis.TtsEngine.ITtsEngineSite)
additional_notes.overrides: *content
---

<p>Custom speech synthesizer implements using <xref href="System.Speech.Synthesis.TtsEngine.TtsEngineSsml"></xref> and <xref href="System.Speech.Synthesis.TtsEngine.TtsEngineSsml.Speak(System.Speech.Synthesis.TtsEngine.TextFragment[],System.IntPtr,System.Speech.Synthesis.TtsEngine.ITtsEngineSite)"></xref> work as filters or intermediaries between synthesizer applications constructed using the platform infrastructure through the members of the <xref href="System.Speech.Synthesis"></xref> namespace and underlying system speech synthesis engines.  
  
 A <xref href="System.Speech.Synthesis.TtsEngine.TtsEngineSsml.Speak(System.Speech.Synthesis.TtsEngine.TextFragment[],System.IntPtr,System.Speech.Synthesis.TtsEngine.ITtsEngineSite)"></xref> implementation:  
  
1.  Traps or modify aspects of the incoming <xref href="System.Speech.Synthesis.TtsEngine.TextFragment"></xref> objects  
  
2.  Generates any necessary events using the site reference to a <xref href="System.Speech.Synthesis.TtsEngine.ITtsEngineSite"></xref> instance  
  
3.  Generates the actual synthesized speech.  
  
 Generation of speech is most typically done by calling <code>Speak</code> on one of the speech rendering engines provided by the operating system.  
  
 If one of the available speech rendering engines is not used, a object inheriting from <xref href="System.Speech.Synthesis.TtsEngine.TtsEngineSsml"></xref> must create its own speech rendering engine.  
  
 Access to the <code>Speak</code> method on obtained using the registry and reflection. .  
  
 When you inherit from <xref href="System.Speech.Synthesis.TtsEngine.TtsEngineSsml"></xref>, you must override the following members: <xref href="System.Speech.Synthesis.TtsEngine.TtsEngineSsml.#ctor(System.String)"></xref>, <xref href="System.Speech.Synthesis.TtsEngine.TtsEngineSsml.AddLexicon(System.Uri,System.String,System.Speech.Synthesis.TtsEngine.ITtsEngineSite)"></xref>, <xref href="System.Speech.Synthesis.TtsEngine.TtsEngineSsml.RemoveLexicon(System.Uri,System.Speech.Synthesis.TtsEngine.ITtsEngineSite)"></xref>, <xref href="System.Speech.Synthesis.TtsEngine.TtsEngineSsml.GetOutputFormat(System.Speech.Synthesis.TtsEngine.SpeakOutputFormat,System.IntPtr)"></xref>, and <xref href="System.Speech.Synthesis.TtsEngine.TtsEngineSsml.Speak(System.Speech.Synthesis.TtsEngine.TextFragment[],System.IntPtr,System.Speech.Synthesis.TtsEngine.ITtsEngineSite)"></xref>.</p>


