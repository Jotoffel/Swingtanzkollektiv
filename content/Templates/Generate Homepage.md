
<%*
const dv = this.app.plugins.plugins["dataview"].api;
const query = 'List Without ID "[["+file.name+"]]" FROM #LindyHop AND #Move WHERE file.name != "Generate Homepage"'

const result = await dv.queryMarkdown(query);

if ( result.successful ) {
 tR += result.value
} else {
  tR += "~~~~\n" + result.error + "\n~~~~"
}
%>
