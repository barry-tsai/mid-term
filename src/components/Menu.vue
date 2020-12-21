<template lang="pug">
.topFlex
	.topMenu
		ul.drop-down-menu
			li
				a(href='#') Home
			li
				a(href='#') 關於學院
				ul
					li
						a(href='#') 學院簡介
					li
						a(href='#') 未來展望
					li
						a(href='#') 姐妹學校
			li
				a(href='#') 學院師資
				ul
					li
						a(href='#') 榮譽院長
					li
						a(href='#') 歷任院長
					li
						a(href='#') 現任院長
					li
						a(href='#') 行政人員
					li
						a(href='#') 專兼任師資
			li
				a(href='#') 學院規章
				ul
					li
						a(href='#') 規章辦法
					li
						a(href='#') 教師評鑑
					li
						a(href='#') 院評鑑
					li
						a(href='#') 會議記錄〉
						ul
							li
								a(href='#') 院務會議
							li
								a(href='#') 院行政會議
							li
								a(href='#') 院課程會議
							li
								a(href='#') 其他會議
			li
				a(href='#') 招生訊息
				ul
					li
						a(href='#') 院學士班(IPTA)
					li
						a(href='#') 音樂系(music)
					li
						a(href='#') 藝設系(art&design)
					li
						a(href='#') 跨院碩(AET)
					li
						a(href='#') 國際交換
			li
				a(href='#') 活動花絮
				ul
					li
						a(href='#') 藝院藝術季
					li
						a(href='#') 國際交流
			li
				a(href='#') 藝院影音
				ul
					li
						a(href='#') 學院影音
					li
						a(href='#') 藝設系影音
					li
						a(href='#') 音樂系影音
			li
				a(href='#') 聯絡資訊
	img.topPhoto(src="http://art.nthu.edu.tw/wp-content/themes/Hector/timthumb.php?src=https://art.nthu.edu.tw/wp-content/uploads/2019/12/%E5%8B%BE%E5%8B%92-%E6%96%B0%E7%AB%B9%E5%9F%8E%E5%B8%82%E7%BE%8E%E8%A1%93%E9%A4%A81127.png&h=400&w=940&zc=1")
	.intFlex
		.intContainer(v-for="item in font")
			.intFont {{item.title}}
			.intSub {{item.sub}}
</template>

<script>
export default {
	name: 'Menu',
	props: {
		msg: String
	},
	data(){
		return{
			font:[
				{title:'院學士班招生-科技藝術', sub:'歡迎你一起來開創清華科技藝術跨域DNA'},
				{title:'藝設系招生-“藝”鳴驚人', sub:'歡迎你一起來把美感、創意帶入清華生活'},
				{title:'音樂系招生-全方位音樂人',sub:'歡迎你一起在清華創造音樂心靈饗宴'}
			]
		}
	}
}
</script>

<style lang="sass">
.topFlex
	display: flex
	flex-direction: column
	background-color: white
	//border: 1px solid red
	position: absolute
	width: 1300px
	height: 1180px
	left: 100px
	top: 100px
	box-shadow: inset 4px 6px 10px 0px rgba(0, 0, 0, 0.5)

.topMenu
	//border: 1px solid blue
	background-color: #EDE7F1
	margin-top: 150px
	margin-left: 40px
	width: 1220px
	height: 66px
	display: flex

.listMenu
	//border: 1px solid orange
	background-color: #EDE7F1
	font-style: normal
	font-weight: normal
	font-size: 30px

ul
	margin: 0
	padding: 0
	list-style: none
	
	&.drop-down-menu
		//border: #ccc 1px solid
		display: inline-block
		font-size: 30px
		font-weight: bold
		line-height: 65px
		
		li
			position: relative
			white-space: nowrap
			//border-right: #ccc 1px solid
		
		> li
			&:last-child
				border-right: none
			
			float: left
		
		a
			background-color: #EDE7F1
			color: #333
			display: block
			padding: 0 18.8px
			text-decoration: none
			line-height: 65px

			&:hover
				opacity: .6
				background-color: #EDE7F1
				color: black

		li:hover > a
			background-color: #6a4c9c
			color: #fff
		
		ul
			//border: #ccc 1px solid
			position: absolute
			z-index: 99
			left: -1px
			top: 100%
			min-width: 162px

			li
				//border-bottom: #ccc 1px solid

				&:last-child
				border-bottom: none

			ul
				/*第三層以後的選單出現位置與第二層不同
				z-index: 999
				top: 0px
				left: 90%

			/*隱藏次選單
			display: none

		li:hover > ul
			/* 滑鼠滑入展開次選單
			display: block

.topPhoto
	//border: 1px solid blue
	margin-left: 40px
	width: 1220px
	height: 705px
	display: flex
	opacity: .9

.intFlex
	display: flex
	background-color: #EDE7F1
	flex-direction: row
	// border: 1px solid red
	justify-content: space-around
	width: 1220px
	height: 210px
	margin-left: 40px

.intContainer
	// border: 1px solid blue
	height: 110px
	display: flex
	margin-top: 50px
	flex-direction: column

.intFont
	// border: 1px solid orange
	width: 400px
	height: 45px
	font-weight: bold
	font-size: 30px
	line-height: 45px

.intSub
	// border: 1px solid green
	width: 400px
	height: 45px
	font-weight: bold
	font-size: 21px
	line-height: 45px
	margin-top: 20px
	color: #63407E

</style>