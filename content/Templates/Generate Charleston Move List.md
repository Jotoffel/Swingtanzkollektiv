## Charleston Moves:
<%*
const dv = this.app.plugins.plugins["dataview"].api;
const query = 'List Without ID "[["+file.name+"]]" FROM #Charleston AND #Move WHERE file.name != "Generate Homepage"'

const result = await dv.queryMarkdown(query);

if ( result.successful ) {
 tR += result.value
} else {
  tR += "~~~~\n" + result.error + "\n~~~~"
}
const query2 = 'List Without ID "[["+file.name+"]]" FROM #LindyHop AND #Move WHERE file.name != "Generate Homepage"'

const result2 = await dv.queryMarkdown(query2);

if ( result2.successful ) {
 tR += result2.value
} else {
  tR += "~~~~\n" + result2.error + "\n~~~~"
}
%>