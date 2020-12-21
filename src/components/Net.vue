<template lang="pug">
.netFlex
    .netColume
        .netColor
            .netFont 學院相關網站
    .blankSpace
    img.netPhoto(src="../assets/Net.jpg")
</template>

<style lang="sass">
.netFlex
	display: flex
	flex-direction: column
	//border: 1px solid red
	position: absolute
	width: 1300px
	height: 580px
	left: 100px
	top: 2930px


.netColume
	// border: 1px solid blue
	margin-top: 50px
	margin-left: 40px
	width: 400px
	height: 66px
	display: flex

.netColor
	// border: 1px solid orange
	background-color: black
	width: 400px
	height: 66px

.netFont
	// border: 1px solid green
	width: 260px
	height: 45px
	font-size: 31px
	line-height: 45px
	margin-top: 10.5px
	color: white

.blankSpace
	//border: 1px solid red
	width: 1220px
	height: 22px
	margin-left: 40px

.netPhoto
	//border: 1px solid blue
	margin-left: 22px
	width: 1270px
	height: 500px
	display: flex

</style>