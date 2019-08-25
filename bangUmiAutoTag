// ==UserScript==
// @name         bangumi TAG
// @namespace    http://tampermonkey.net/
// @version      0.1
// @description  try to take over the world!
// @author       You
// @include      /^https?://(bangumi\.tv|bgm\.tv|chii\.in)/update/.*
// @grant        none
// ==/UserScript==

(function() {
    'use strict';
    var inner = document.querySelectorAll(".inner");
    var arr1 = inner[0].innerText.split("\n");
    var arr2 = inner[1].innerText.split("\n");
    console.log({arr1,arr2});
    var res = arr1.filter(i => getTag(i));
    let tagStr = res.join(" ");
    function getTag(tag){
        if(tag == "")return false;
    	console.log(arr2.indexOf(tag)!=-1);
    	return arr2.indexOf(tag)!=-1;
    };
    chiiLib.subject.addTag(tagStr);

    // Your code here...
})();
