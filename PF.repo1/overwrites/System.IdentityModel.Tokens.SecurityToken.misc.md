---
uid: System.IdentityModel.Tokens.SecurityToken
additional_notes.overrides: *content
---

<p>You must override the <xref href="System.IdentityModel.Tokens.SecurityToken.Id"></xref>, <xref href="System.IdentityModel.Tokens.SecurityToken.SecurityKeys"></xref>, <xref href="System.IdentityModel.Tokens.SecurityToken.ValidFrom"></xref>, and <xref href="System.IdentityModel.Tokens.SecurityToken.ValidTo"></xref> properties. The <xref href="System.IdentityModel.Tokens.SecurityToken.CanCreateKeyIdentifierClause``1"></xref>, <xref href="System.IdentityModel.Tokens.SecurityToken.CreateKeyIdentifierClause``1"></xref>, <xref href="System.IdentityModel.Tokens.SecurityToken.MatchesKeyIdentifierClause(System.IdentityModel.Tokens.SecurityKeyIdentifierClause)"></xref>, and <xref href="System.IdentityModel.Tokens.SecurityToken.ResolveKeyIdentifierClause(System.IdentityModel.Tokens.SecurityKeyIdentifierClause)"></xref> methods all support key identifiers of type <xref href="System.IdentityModel.Tokens.LocalIdKeyIdentifierClause"></xref>. You must override these methods to support other key identifier types in your derived class.</p>


