Sistem Informasi Geografis – OpenLay

1. Latar Belakang

Dalam pembahasan Sistem Informasi Geografis kali ini, akan dibahas tentang Overlay. Untuk lebih jelasnya akan dibahas dalam pembahasan.

1. Pembahasan

1. OpenLayers adalah library Javascript murni untuk menampilkan data peta di berbagai web browser, tanpa server side dependencies. Openlayers mengimplementasikan JavaScript API untuk membangun rich web-based geographic aplication yang mirip dengan Geoogle maps dan MSN Virtual Earth APIS.
2. Overlay adalah kemampuan untuk menempatkan grafis satu peta diatas grafis peta yang lain dan menampilkan di layar komputer atau pada plot.
3. Contoh Overlay dan OpenLayer

		<!DOCTYPE html>
	<html>
	  <head>
	    <title>Overlay</title>
	    <link rel="stylesheet" href="https://openlayers.org/en/v3.20.1/css/ol.css" type="text/css">
	    <!-- The line below is only needed for old environments like Internet Explorer and Android 4.x -->
	    <script src="https://cdn.polyfill.io/v2/polyfill.min.js?features=requestAnimationFrame,Element.prototype.classList,URL"></script>
	    <script src="https://openlayers.org/en/v3.20.1/build/ol.js"></script>
	    <script src="https://code.jquery.com/jquery-2.2.3.min.js"></script>
	    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css">
	    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/js/bootstrap.min.js"></script>
	    <style>
	      #marker {
	        width: 20px;
	        height: 20px;
	        border: 1px solid #088;
	        border-radius: 10px;
	        background-color: #FF3300;
	        opacity: 0.5;
	      }
	      #marker2 {
	        width: 20px;
	        height: 20px;
	        border: 1px solid #088;
	        border-radius: 10px;
	        background-color: #FF3300;
	        opacity: 0.5;
	      }
	      #marker3 {
	        width: 20px;
	        height: 20px;
	        border: 1px solid #088;
	        border-radius: 10px;
	        background-color: #FF3300;
	        opacity: 0.5;
	      }
	      #marker4 {
	        width: 20px;
	        height: 20px;
	        border: 1px solid #088;
	        border-radius: 10px;
	        background-color: #FF3300;
	        opacity: 0.5;
	      }
	      #marker5 {
	        width: 20px;
	        height: 20px;
	        border: 1px solid #088;
	        border-radius: 10px;
	        background-color: #FF3300;
	        opacity: 0.5;
	      }
	      #bandung {
	        text-decoration: none;
	        color: black;
	        font-size: 11pt;
	        font-weight: bold;
	        text-shadow: white 0.1em 0.1em 0.2em;
	      }
	      #meulaboh {
	        text-decoration: none;
	        color: black;
	        font-size: 11pt;
	        font-weight: bold;
	        text-shadow: white 0.1em 0.1em 0.2em;
	      }
	      #tapaktuan {
	        text-decoration: none;
	        color: black;
	        font-size: 11pt;
	        font-weight: bold;
	        text-shadow: white 0.1em 0.1em 0.2em;
	      }
	      #binjai {
	        text-decoration: none;
	        color: black;
	        font-size: 11pt;
	        font-weight: bold;
	        text-shadow: white 0.1em 0.1em 0.2em;
	      }
	      #lhokseumawe {
	        text-decoration: none;
	        color: black;
	        font-size: 11pt;
	        font-weight: bold;
	        text-shadow: white 0.1em 0.1em 0.2em;
	      }
	      .popover-content {
	        min-width: 180px;
	      }
	    </style>
	  </head>

