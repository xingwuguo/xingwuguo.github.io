郭兴伍 博士

上海市闵行区东川路800号 <br/>
上海交通大学材料科学与工程学院 <br/>
Tel: +86-21-54745091 <br/>
Mobile: +86-137-7427-6195 <br/>
Email: xingwuguo@sjtu.edu.cn

<script src="https://api.map.baidu.com/api?v=2.0&ak=1a3c89ddb9bcfaf5b9dc4b62e3f2a05b"></script>
/* Create two columns that float next to eachother */
.column {
    float: left;
    width: 50%;
    margin-top: 6px;
    padding: 20px;
}

/* Clear floats after the columns */
.row:after {
    content: "";
    display: table;
    clear: both;
}


// 百度地图API功能
  var map = new BMap.Map("allmap");    // 创建Map实例
  map.centerAndZoom(new BMap.Point(116.404, 39.915), 11);  // 初始化地图,设置中心点坐标和地图级别
  //添加地图类型控件
  map.addControl(new BMap.MapTypeControl({
    mapTypes:[
            BMAP_NORMAL_MAP,
            BMAP_HYBRID_MAP
        ]}));   
  map.setCurrentCity("上海交通大学");          // 设置地图显示的城市 此项是必须设置的
  map.enableScrollWheelZoom(true);     //开启鼠标滚轮缩