<template lang="pug">
.actFlex
    .actColume
        .actColor
            .actFont 近期活動
    .blankSpace
    .actFrame
        .actList(v-for='item in detail')
            .actDate {{item.date}}
            .actDetail {{item.describe}}
</template>

<script>
export default {
	name: 'Menu',
	props: {
		msg: String
	},
	data(){
		return{
			detail:[
				{date:'2020/12/08', describe:'藝設系學生獲獎－109年林務局「國產材設計商品比賽」決選'},
				{date:'2020/12/01', describe:'2021 年藝術學院教育發展基金'},
				{date:'2020/12/01', describe:'【開放報名】2020國立清華大學藝術與設計學系研究生論文研討會'},
				{date:'2020/09/24', describe:'清華大學藝設系研究生論文研討會–徵稿'},
				{date:'2020/09/09', describe:'ARS 2020–Tsing Hua Garden'},
				{date:'2020/07/31', describe:'清華藝術學報'},
				{date:'2020/07/22', describe:'藝設系設計組-異質對話-（360展區1）'},
				{date:'2020/07/03', describe:'華山烏梅劇場「Face to face」實驗性跨領域展演 × 四組劇場表演與一組互動裝置'}
			]
		}
	}
}
</script>

<style lang="sass">
.actFlex
	display: flex
	flex-direction: column
	background-color: white
	// border: 1px solid red
	position: absolute
	width: 1300px
	height: 2150px
	left: 100px
	top: 1400px
	box-shadow: inset 7px 0px 10px -2px rgba(0, 0, 0, 0.5)

.actColume
	// border: 1px solid red
	margin-top: 50px
	margin-left: 40px
	width: 400px
	height: 66px
	display: flex

.actColor
	// border: 1px solid orange
	background-color: black
	width: 400px
	height: 66px

.actFont
	// border: 1px solid green
	width: 200px
	height: 45px
	font-size: 31px
	line-height: 45px
	margin-top: 10.5px
	color: white

.blankSpace
	//border: 1px solid red
	width: 1220px
	height: 40px
	margin-left: 40px

.actFrame
	display: flex
	background-color: #E5E5E5
	flex-direction: column
	// border: 3px solid red
	width: 1220px
	height: 1330px
	margin-left: 40px
	box-shadow: 7px 7px 20px 1px rgba(0, 0, 0, 0.2)

.actList
	margin-top: 10px 
	justify-content: center
	// border: 3px solid blue
	margin-right: 30px 
	height: 150px
	display: flex
	flex-direction: column

.actDate
	// border: 3px solid yellow
	width: 300px
	height: 45px
	font-size: 30px
	font-weight: bold
	line-height: 45px

.actDetail
	//border: 3px solid orange
	height: 66px
	display: flex
	font-size: 30px
	font-weight: bold
	line-height: 45px
	margin-left: 260px
	text-align: left
</style>