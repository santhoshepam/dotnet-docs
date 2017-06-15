---
summary: Encrypts the key that a recipient uses to decrypt an `<EncryptedData>` element.
remarks: Use the <xref:System.Security.Cryptography.Xml.EncryptedXml.EncryptKey%2A> method to encrypt the key that a recipient uses to decrypt an `<EncryptedData>` element. This method places the encrypted key within an `<EncryptedKey>` element.
example:
- "The following code example demonstrates how to encrypt an XML document using an asymmetric key. This example creates a symmetric session key to encrypt the document and then uses the asymmetric key to embed an encrypted version of the session key into the XML document.  \n  \n [!code-cpp[Cryptography.XML.XMLEncImbedKey#1](~/samples/snippets/cpp/VS_Snippets_CLR/Cryptography.XML.XMLEncImbedKey/CPP/sample.cpp#1)]\n [!code-csharp[Cryptography.XML.XMLEncImbedKey#1](~/samples/snippets/csharp/VS_Snippets_CLR/Cryptography.XML.XMLEncImbedKey/CS/sample.cs#1)]\n [!code-vb[Cryptography.XML.XMLEncImbedKey#1](~/samples/snippets/visualbasic/VS_Snippets_CLR/Cryptography.XML.XMLEncImbedKey/VB/sample.vb#1)]"
uid: System.Security.Cryptography.Xml.EncryptedXml.EncryptKey*
---
