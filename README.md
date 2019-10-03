# youtube export channel 
youtube channel video export

In browser console add this

var jq = document.createElement('script');
jq.src = "https://ajax.googleapis.com/ajax/libs/jquery/2.1.4/jquery.min.js";
document.getElementsByTagName('head')[0].appendChild(jq);
// ... give time for script to load, then type (or see below for non wait option)
jQuery.noConflict();

// and this

jQuery('ytd-grid-video-renderer').each(function (index, value) {
href = jQuery(this).find('a').attr('href');
title = jQuery(this).find('#video-title').text();
console.log(href +"#"+ title);

});
