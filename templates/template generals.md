---
<%*
  let title = tp.file.title
  {
    title = await tp.system.prompt("Title");
    await tp.file.rename(title);
  } 
  
  tR += "---"
%>
file:  <% tp.file.folder() %>\<%* tR += title %>
created: <% tp.file.creation_date() %> modified: <% tp.file.last_modified_date("dddd Do MMMM YYYY HH:mm") %>

Tags:

title: ""
date: <% tp.file.creation_date("YYYY-MM-DDT:HH:MM:ss:ss") %>
draft: false
---
  # Header