
<%*
const dv = this.app.plugins.plugins["dataview"].api;
const query = 'LIST FROM #LindyHop AND #Move WHERE file.name != "Generate Homepage"';
const result = await dv.queryMarkdown(query);

if ( result.successful ) {
 tR += result.value
} else {
  tR += "~~~~\n" + result.error + "\n~~~~"
}
%>
