# RT_4_Tonenchuk
<html xmlns="http://www.w3.org/1999/xhtml"> 
<head>     <title>Примеры. Добавление прямоугольника на карту.</title>  
   <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/> 
 <script src="http://api-maps.yandex.ru/2.0/?load=package.full&lang=ru-RU"            
         type="text/javascript"></script> 
  <script type="text/javascript">
 ymaps.ready(init); 
 function init() { 
 var myMap = new ymaps.Map('map', { 
  center: [-22.139066, 17.222231], 
 zoom: 8
 }), 
  myRect = new ymaps.Rectangle([ 
   [-22.217612, 16.707263], 
  [-22.91654, 17.520247] 
 ]), 
 myGeoObject = new ymaps.GeoObject({ 
 geometry: { 
 type: "Rectangle", 
 coordinates: [ 
  [-22.217612, 16.707263], 
  [-22.91654, 17.520247]  
 ] 
 } 
 }); 
  myMap.geoObjects.add(myRect) 
 .add(myGeoObject); 
   } 
 </script> 
</head> 
<body> 
<h2>Добавление прямоугольника на карту</h2> 	
<div id="map" style="width:600px;height:400px"></div> 
</body> 
</html> 
