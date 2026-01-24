Xingwu Guo, Ph.D.

School of Materials Science and Engineering  
Shanghai Jiao Tong University   
800 Dongchuan Road, Shanghai, China  
Tel: +86-21-54745091  
Mobile: +86-137-7427-6195  
Email: xingwuguo@sjtu.edu.cn

<script type="text/javascript" src="https://api.map.baidu.com/api?v=2.0&ak={{ site.baidu_map_ak }}"></script>

<div style="width:100%; max-width:1000px; height:400px; border:1px solid #ccc; margin-top:15px;" id="container"></div>

<script type="text/javascript">
    // Create map instance
    var map = new BMap.Map("container");
    // Initialize map with center coordinates and zoom level
    map.centerAndZoom(new BMap.Point(121.433845,31.028902), 18);
    // Add map controls
    map.addControl(new BMap.NavigationControl());
    map.addControl(new BMap.ScaleControl());
    map.addControl(new BMap.OverviewMapControl());
    // Set the current city (required)
    map.setCurrentCity("上海");
    // Enable scroll wheel zoom
    map.enableScrollWheelZoom(true);
</script>