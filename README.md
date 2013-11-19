图片展示插件：

开发技术点 1：图片预计加载
          
           2：刷新页面停留当前页
           
默认餐数：
       
bdUI.dullImgShow.defaults = {

		//图片标题
		titleName: '#title-name',
		
		//当前序号
		currentSort: '#current-num',
		
		//总共张数
		sum: '.main-title-all',
		
		//图片展示盒子
		bigBox: '#big-ul',
		
		//大图下一张按钮
		bigNext: '#big-next',
		
		//大图上一张按钮
		bigPrev: '#big-prev',
		
		//缩略图滚动盒子
		smallBox: '#small-ul',
		
		//缩略图下一张按钮
		smallNext: '#small-next',
		
		//缩略图上一张按钮
		smallPrev: '#small-prev',
		
		//最后一张回调函数
		overcallback: null,
		
		//点击缩略图回调函数
		closedcallback: null
}

实例化：

$('.main-pic-show').dullImgShow({
    'overcallback':function(){
     		$('.main-dialog').show();
     		$('.main-shade').show();
     },
     'closedcallback':function(){
        	$('.main-dialog').hide();
        	$('.main-shade').hide();        	
     }
});
