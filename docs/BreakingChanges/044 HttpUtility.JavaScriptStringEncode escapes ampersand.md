## 44: HttpUtility.JavaScriptStringEncode escapes ampersand

### Scope
Minor

### Version Introduced
4.5

### Change Description
Starting with the .NET Framework 4.5, JavaScriptStringEncode escapes the ampersand (&amp;) character.

- [ ] Quirked
- [ ] Build-time break
- [x] Source analyzer available

### Recommended Action
If your app depends on the previous behavior of this method, you can add an aspnet:JavaScriptDoNotEncodeAmpersand setting to the [ASP.NET appSettings element](https://msdn.microsoft.com/en-us/library/hh975440(v=vs.110).aspx) in your configuration file.

### Affected APIs
* `M:System.Web.HttpUtility.JavaScriptStringEncode(System.String)`
* `M:System.Web.HttpUtility.JavaScriptStringEncode(System.String,System.Boolean)`

[More information](https://msdn.microsoft.com/en-us/library/hh367887(v=vs.110).aspx#asp)