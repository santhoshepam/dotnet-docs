---
summary: Returns the collection of speech synthesis (text-to-speech) voices that are currently installed on the system.
remarks: When an application calls <xref:System.Speech.Synthesis.SpeechSynthesizer.GetInstalledVoices%2A>, the method verifies that each of the voices (engines for text-to-speech) it finds in the registry meets certain minimum criteria. For any voice that fails verification, <xref:System.Speech.Synthesis.SpeechSynthesizer.GetInstalledVoices%2A> sets its <xref:System.Speech.Synthesis.InstalledVoice.Enabled%2A> property to `False`. An application cannot select a voice whose <xref:System.Speech.Synthesis.InstalledVoice.Enabled%2A> property is `False`. Typically, applications will not set a voice’s <xref:System.Speech.Synthesis.InstalledVoice.Enabled%2A> property.
uid: System.Speech.Synthesis.SpeechSynthesizer.GetInstalledVoices*
---
