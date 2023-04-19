---
title: ipsum faucibus vitae 1
date: 2022-01-28T15:53:12.000Z
draft: true
tags: [Bikes]
categories: [Road bikes]
weight: 1
description: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ac ultricies sem, id luctus tortor. Nam tincidunt felis nec fringilla ullamcorper. Aenean congue lacus ut ipsum tempus, et lacinia nisi suscipit. Nulla pellentesque ante vitae leo efficitur, ut porta turpis tempus. Vivamus imperdiet urna eu nunc maximus semper.
---

## Tabs + Syntax Highlighter + Code Copy
{{< tabpane text=true right=false >}}
  {{% tab header="**YAML**:" %}}
```yaml
	books:
	- name: The Hate U Give
	  author: Angie Thomas
	  pages: 392
	  publisher: Balzer + Bray
	  date_read: 2020-03-23
	  fiction: yes
	  female_author: yes
	  rating: 5
	- name: Good Book
	  author: Uncle Sam
	  pages: 100
	  publisher: Cisco Press
	  date_read: 2023-03-23
	  fiction: yes
	  female_author: yes
	  rating: 4

```
  {{% /tab %}}
  {{% tab header="**XML**"  %}}
```xml

<!DOCTYPE glossary PUBLIC "-//OASIS//DTD DocBook V3.1//EN">
 <glossary><title>example glossary</title>
  <GlossDiv><title>S</title>
   <GlossList>
    <GlossEntry ID="SGML" SortAs="SGML">
     <GlossTerm>Standard Generalized Markup Language</GlossTerm>
     <Acronym>SGML</Acronym>
     <Abbrev>ISO 8879:1986</Abbrev>
     <GlossDef>
      <para>A meta-markup language, used to create markup languages such as DocBook.</para>
      <GlossSeeAlso OtherTerm="GML">
      <GlossSeeAlso OtherTerm="XML">
     </GlossDef>
     <GlossSee OtherTerm="markup">
    </GlossEntry>
   </GlossList>
  </GlossDiv>
 </glossary>
```
  {{% /tab %}}
  {{% tab header="**Markdown**"  %}}
```markdown
 
 Help your user know if your project will help them. Useful information can include: 

-   **What is it good for?**: What types of problems does your project solve? What are the benefits of using it?

-   **What is it not good for?**: For example, point out situations that might intuitively seem suited for your project, but aren't for some reason. Also mention known limitations, scaling issues, or anything else that might let your users know if the project is not for them.

-   **What is it _not yet_ good for?**: Highlight any useful features that are coming soon.
```
  {{% /tab %}}
  {{% tab header="**HTML**"  %}}
```html
 <li class="li">
   <p class="p">
      <span class="ph uicontrol">Impacted Firmware/Version</span>—The software version of UCS systems impacted.
   </p>
</li>
<li class="li">
   <p class="p">
      <span class="ph uicontrol">Effective Date</span>—Date when the EOL advisory milestone is reached. As an example, for UCS Manager Release 2.2 the effective date is either the date when the EOSM milestone of January 9, 2019 was reached or LDOS milestone is January 31, 2023 was reached.
   </p>
</li>
```
  {{% /tab %}}
{{% /tabpane %}}

## Cards

### Card Panes

{{< card-code header="**C**" lang="C" >}}
\#include &lt;stdio.h>
\#include &lt;stdlib.h>

int main(void)
{
  puts("Hello World!");
  return EXIT_SUCCESS;
}
{{< /card-code >}}

<HR>

{{< card header="**Imagine**" title="Artist and songwriter: John Lennon" subtitle="Co-writer: Yoko Ono" footer="![SignatureJohnLennon](https://marinegeo.github.io/assets/img/MarineGEO_logo.png 'Signature John Lennon')" >}}
Imagine there's no heaven, It's easy if you try<br/>
No hell below us, above us only sky<br/>
Imagine all the people living for today...

...
{{< /card >}}

### Card Group

{{< cardpane >}}
  {{< card header="**Card 1**" >}}
    Content card 1
  {{< /card >}}
  {{< card header="**Card 2**" >}}
    Content card 2
  {{< /card >}}
  {{< card header="**Card 3**" >}}
    Content card 3
  {{< /card >}}
{{< /cardpane >}}

## Hightlight

### Warning

{{% alert title="Warning" color="warning" %}}
This is a warning.
{{% /alert %}}

### Note

{{% alert title="Note" %}}
This is a Note.
{{% /alert %}}

### Tip

{{% alert title="Tip" %}}
This is a Tip.
{{% /alert %}}

## Content Resuse and Conditional Tag Shortcodes

### Include External File

The following section explains how to install the database:

{{% readfile "NewFeatures2.md" %}}

### Include a code snippet (External File)

To create a new pipeline, follow the next steps:

1.  Create a configuration file `config.yaml`:

    {{< readfile file="config.yaml" code="true" lang="yaml" >}}

2.  Apply the file to your cluster `kubectl apply config.yaml`

### Conditional Tag Processing

{{% conditional-text include-if="foo" %}}
This text appears in the output only if `buildCondition = "foo" is set in your config file`.
{{% /conditional-text %}}
{{% conditional-text exclude-if="bar" %}}
This text does not appear in the output if `buildCondition = "bar" is set in your config file`.
{{% /conditional-text %}}

## Blocks

{{< blocks/section color="dark" type="row" >}}
{{% blocks/feature icon="fa-lightbulb" title="Fastest OS **on the planet**!" %}}
The new **TechOS** operating system is an open source project. It is a new project, but with grand ambitions.
Please follow this space for updates!
{{% /blocks/feature %}}
{{% blocks/feature icon="fa-brands fa-github" title="Contributions welcome!" url="https://github.com/gohugoio/hugo" %}}
We do a [Pull Request](https://github.com/gohugoio/hugo/pulls) contributions workflow on **GitHub**. New users are always welcome!
{{% /blocks/feature %}}
{{% blocks/feature icon="fa-brands fa-twitter" title="Follow us on Twitter!" url="https://twitter.com/GoHugoIO" %}}
For announcement of latest features etc.
{{% /blocks/feature %}}
{{< /blocks/section >}}

## swaggerui

{{< swaggerui src="https://github.com/OAI/OpenAPI-Specification/blob/main/examples/v2.0/yaml/petstore.yaml" >}}

## redoc

{{< redoc "https://raw.githubusercontent.com/OAI/OpenAPI-Specification/main/examples/v2.0/yaml/petstore.yaml" >}}
