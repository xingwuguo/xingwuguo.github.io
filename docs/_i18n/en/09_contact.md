Xingwu Guo, Ph.D.

School of Materials Science and Engineering  
Shanghai Jiao Tong University   
800 Dongchuan Road, Shanghai, China  
Tel: +86-21-54745091  
Mobile: +86-137-7427-6195  
Email: xingwuguo@sjtu.edu.cn

<script type="text/javascript" src="https://api.map.baidu.com/api?v=2.0&ak=1a3c89ddb9bcfaf5b9dc4b62e3f2a05b"></script>

<div style="width:1000px; height:400px; borders:1px; margin-top:15px;" id="container"></div>

<script type="text/javascript">
    <!-- // 创建地图实例  -->
    var map = new BMap.Map("container");  
    <!-- // 初始化地图,设置中心点坐标和地图级别 -->
    map.centerAndZoom(new BMap.Point(121.433845,31.028902), 17);
    <!-- // 添加地图类型控件 -->
    map.addControl(new BMap.NavigationControl())
    map.addControl(new BMap.ScaleControl())
    map.addControl(new BMap.OverviewMapControl())
    var local=new BMap.LocalSearch(map,{renderOptions:{map:map}})
    local.seach("上海交通大学")
    <!-- // 设置地图显示的城市 此项是必须设置的 -->
    map.setCurrentCity("上海"); 
    <!-- // 开启鼠标滚轮缩 -->
    map.enableScrollWheelZoom(true);
</script>