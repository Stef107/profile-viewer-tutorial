# profile-viewer-tutorial (add note)  

https://taisukef.github.io/profile-viewer-tutorial/  
Japanese ver.  

https://taisukef.github.io/profile-viewer-tutorial/index_en.html  
English ver.  

# to add note  

index.html  
&lt;dt&gt;Note&lt;/dt&gt;&lt;dd id="note"&gt;&lt;/dd&gt;  

main.js  
const VCARD = $rdf.Namespace('http://www.w3.org/2006/vcard/ns#');  
// Display their note (added by taisukef)  
const note = store.any($rdf.sym(person), VCARD('note'));  
$('#note').text(note && note.value);  
