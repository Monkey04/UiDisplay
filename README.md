#UiDisplay
用于结构化展示Ui设计图的小模块


> 使用方法：
> 修改data.js文件中的sourceData变量

    var sourceData={
	menu_width:null,//左边菜单总宽度，最低不能低于170px，默认为200px
	data:[{
		text:"首页",
		img:"img/test4.jpg",
	},{
		text:"会员中心",
		img:"",
		sub:[{
			text:"会员注册",
			img:"img/test2.jpg",
			sub:[]
		},{
			text:"会员登录",
			img:"img/test1.jpg"
		},{
			text:"会员信息",
			img:"",
			sub:[{
				text:"基本信息",
				img:"none",
		        sub:[]
			},{
				text:"进阶信息",
				img:"img/test3.jpg",
		        sub:[]
			},{
				text:"高级信息",
				img:"",
				sub:[]
			}]
		}]
	}]
	}
> sourceData.data所有子对象都由text,img,sub参数组成，img和sub非必要，用以构建左侧结构树形式的菜单
