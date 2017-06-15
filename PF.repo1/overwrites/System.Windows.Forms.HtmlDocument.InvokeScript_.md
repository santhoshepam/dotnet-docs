---
summary: Executes an Active Scripting function defined in an HTML page.
example:
- "The following code example executes the contents of a script in a Web page. The code example requires that you have loaded the following Web page.  \n  \n```  \n<HTML>  \n<SCRIPT>  \nfunction test(name, address) {  \nwindow.alert(\"Name is \" + name + \"; address is \" + address);  \n}  \n</SCRIPT>  \n  \n<BODY>  \n</BODY>  \n</HTML>  \n  \n```  \n  \n [!code-csharp[System.Windows.Forms.HtmlDocument#9](~/samples/snippets/csharp/VS_Snippets_Winforms/System.Windows.Forms.HtmlDocument/CS/Form1.cs#9)]\n [!code-vb[System.Windows.Forms.HtmlDocument#9](~/samples/snippets/visualbasic/VS_Snippets_Winforms/System.Windows.Forms.HtmlDocument/VB/Form1.vb#9)]"
uid: System.Windows.Forms.HtmlDocument.InvokeScript*
---
