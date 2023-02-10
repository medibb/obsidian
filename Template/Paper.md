


# **Title: [[<%tp.file.title%>]]**
---

Year: {{date | format("YYYY")}}

tags: zotero

Authors: {{authors}}{{directors}}

---

​

Title:: {{title}}

URL: {{url}}

Zotero Link: {{pdfZoteroLink}}

​

{% for annotation in annotations %}

{%- if annotation.annotatedText -%}

{{annotation.annotatedText}}"{% if annotation.color %}

{{annotation.colorCategory}} {{annotation.type | capitalize}} {% else %}

{{annotation.type | capitalize}} {% endif %}[Page {{annotation.page}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}})

{% endif %}

{%- if annotation.imageRelativePath -%}

![[{{annotation.imageRelativePath}}]]

{%- endif %}

{% if annotation.comment %}

{{annotation.comment}}

{% endif %}[Page {{annotation.page}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}})

{% endfor -%}






🔗LINKS TO THIS PAGE