---

Year: {{date | format("YYYY")}}
Authors: {{authors}}{{directors}}
Title:: {{title}}
URL: {{url}}
Zotero Link: {{pdfZoteroLink}}
tags: zotero

---



# text
{% for annotation in annotations %}
{%- if annotation.annotatedText -%}
{{annotation.annotatedText}}"{% if annotation.color %}
{{annotation.colorCategory}} {{annotation.type | capitalize}} {% else %}
{{annotation.type | capitalize}} {% endif %}[Page {{annotation.page}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}})

# img

{% for annotation in annotations %}
{%- if annotation.imageRelativePath -%}
![[{{annotation.imageRelativePath}}]]


# cmt

{% for annotation in annotations %}
{% if annotation.comment %}
{{annotation.comment}}
{% endif %}[Page {{annotation.page}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}})
{% endfor -%}